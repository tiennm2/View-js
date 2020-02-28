<template>
  <div class="content-header">
    <div class="container-fluid">
      <div class="row mb-2">
        <div class="col-sm-6">
          <h1 class="m-0 text-dark">管理者一覧</h1>
        </div><!-- /.col -->
      </div><!-- /.row -->

      <!-- Main content -->
      <section class="content">
        <div class="row pt-2">
          <div class="col-md-12">
            <button type="button" class="btn btn-contact t-label pl-4 pr-4" data-toggle="modal"
                    data-target="#modal_register_user" id="create-new-manager">
              新規管理者登録
            </button>
          </div>

        </div>
        <div class="card mt-3">
          <div class="card-body">
            <div class="box">
              <div class="box-body">
                <div class="row">
                  <div class="col-12">
                    <table class="table table-bordered table-hover table-custom" id="list-master-admin">
                      <thead>
                      <tr>
                        <th>
                          No
                        </th>
                        <th class="w25percent">
                          ログインID
                        </th>
                        <th class="w25percent">
                          名前
                        </th>
                        <th class="w25percent">
                          最終ログイン日
                        </th>
                        <th class="w25percent">
                          登録日
                        </th>
                        <th class="w25percent text-center">
                          アクション
                        </th>
                      </tr>
                      </thead>
                      <tbody>
                      <tr>
                        <td>1</td>
                        <td>admin</td>
                        <td>manhtien98</td>
                        <td>2020/02/14</td>
                        <td>2020/02/14</td>
                        <td width="15%" class="">
                          <div class="row">
                            <div class="col-md-12">
                              <a href="javascript:void(0)">
                                <button class="btn btn-action btn-edit t-label btn-edit-master mb-2"
                                        data-toggle="modal"
                                        data-target="#modal_register_user"
                                        data-id=""
                                        onclick=""
                                >
                                  編集
                                </button>
                              </a>
                              <a href="javascript:void(0)">
                                <button class="btn btn-action btn-delete t-label btn-delete-master mb-2"
                                        data-toggle="modal"
                                        data-target="#modal_delete_master"
                                        data-id="">
                                  削除
                                </button>
                              </a>
                            </div>
                          </div>
                        </td>

                      </tr>
                      </tbody>
                    </table>
                  </div>
                </div>

              </div>
            </div>
          </div>
        </div>

      </section>
    </div><!-- /.container-fluid -->
    <!--modal register user-->
    <div class="modal fade" id="modal_register_user">
      <div class="modal-dialog modal-dialog-reservation">
        <div class="modal-content" style="background-color: #ffffff">
          <form id="manager-form" action="/" method="post">
            <!--{!! csrf_field() !!}-->
            <div class="modal-body container">
              <input type="hidden" name="id" id="user_id" class="form-control">
              <div class="row">
                <label for="login_id" class="t-label col-12">ログインID <span
                  class="text-danger">*</span></label>
              </div>
              <div class="row">
                <div class="col-12">
                  <input type="text" class="form-control" id="login_id" name="login_id" value="">
                </div>
              </div>
              <div class="row">
                <label for="name" class="t-label col-12">名前<span
                  class="text-danger">*</span></label>
              </div>
              <div class="row">
                <div class="col-12">
                  <input type="text" class="form-control" id="name" name="user_name" value="">
                </div>
              </div>
              <div class="row">
                <label for="pw" class="t-label col-12">パスワード<span
                  class="text-danger" id="span-pw">*</span></label>
              </div>
              <div class="row">
                <div class="col-12">
                  <input type="password" class="form-control" id="pw" name="password" required
                         value="">
                </div>
              </div>
            </div>
            <div class="modal-footer row text-center">
              <div class="col-md-12 m-auto">
                <button type="submit" class="btn btn-custom mr-2 btn-submit">
                  登録
                </button>
                <button type="button" class="btn btn-cancel btn-cancel-add-master" data-dismiss="modal">
                  キャンセル
                </button>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
    <!--end modal register reservation-->
  </div>
</template>

<script>
  export default {
    name: "List",
    data(){
      return{
        users: [
          {}
        ]
      }
    },
  }
</script>

<style scoped>

</style>
