<template>
  <div class="input-file-part">
    <div class="field is-horizontal">
      <div class="field-label is-normal">
        <label class="label">入力ファイル</label>
      </div>
      <div class="field-body">
        <div class="field">
          <div class="file has-name is-fullwidth">
            <label class="file-label">
              <input class="file-input" type="file" name="resume" />
              <span class="file-cta">
                <span class="file-icon">
                  <i class="fas fa-upload"></i>
                </span>
                <span class="file-label">Choose a file…</span>
              </span>
              <span class="file-name">Screen Shot 2017-07-29 at 15.54.25.png</span>
            </label>
          </div>
        </div>
      </div>
    </div>
    <div class="field is-horizontal">
      <div class="field-label is-normal">
        <label class="label">対象列名</label>
      </div>
      <div class="field-body">
        <div class="field is-narrow">
          <div class="control">
            <div class="select is-fullwidth">
              <select>
                <option>Business development</option>
                <option>Marketing</option>
                <option>Sales</option>
              </select>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
div.input-file-part {
  margin-bottom: 20px;
}
</style>