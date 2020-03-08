<template>
  <div>
    <template>
      <div class="section">
        <h1 class="title">Clustering</h1>
        <hr />
        <InputFile />
        <div class="field is-horizontal">
          <div class="field-label is-normal">
            <label class="label">クラスタ数</label>
          </div>
          <div class="field-body">
            <div class="field">
              <div class="control">
                <input class="input" type="number" v-model="n_cluster" />
              </div>
            </div>
          </div>
        </div>
        <div class="field is-horizontal">
          <div class="field-label">
            <label class="label">Already a member?</label>
          </div>
          <div class="field-body">
            <div class="field is-narrow">
              <div class="control">
                <label class="radio">
                  <input type="radio" name="member" />
                  Yes
                </label>
                <label class="radio">
                  <input type="radio" name="member" />
                  No
                </label>
              </div>
            </div>
          </div>
        </div>
        <div class="field">
          <details>
            <summary>詳細設定</summary>
            <div class="field is-horizontal">
              <div class="field-label is-normal">
                <label class="label">ストップワード</label>
              </div>
              <div class="field-body">
                <div class="field">
                  <div class="control">
                    <textarea class="textarea" placeholder="Explain how we can help you"></textarea>
                  </div>
                </div>
              </div>
            </div>
            <div class="field is-horizontal">
              <div class="field-label is-normal">
                <label class="label">類義語</label>
              </div>
              <div class="field-body">
                <div class="field">
                  <div class="control">
                    <textarea class="textarea" placeholder="Explain how we can help you"></textarea>
                  </div>
                </div>
              </div>
            </div>
          </details>
        </div>
        <div class="field is-horizontal">
          <div class="field-label">
            <!-- Left empty for spacing -->
          </div>
          <div class="field-body">
            <div class="field">
              <div class="control">
                <button class="button is-primary">Send message</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </template>
  </div>
</template>

<script>
import InputFile from "~/components/InputFile.vue";

export default {
  components: {
    InputFile
  },
  data() {
    return {
      n_cluster: 1
    };
  }
};
</script>