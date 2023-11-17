<script setup lang="ts">
import { ref } from 'vue';
import type { Ref } from 'vue';

const projectNumber: Ref<string | number> = ref('GD12345')
</script>

<template>
  <form class="box">
    <div class="field is-horizontal">
      <div class="field-label is-normal">
        <label class="label">Project Number</label>
      </div>
      <div class="field-body">
        <div class="field is-grouped">
          <p class="control is-expanded">
            <input class="input" type="email" placeholder="Project Number" v-model="projectNumber">
          </p>
          <p class="control">
            <a class="button is-info">
              Get Sections
            </a>
          </p>
        </div>
      </div>
    </div>
    
    <div class="field is-horizontal">
      <div class="field-label is-normal">
        <label class="label">Sections</label>
      </div>
      <div class="field-body">
        <div class="control">
          <div class="select is-fullwidth">
            <select name="sections">
              <option value="Argentina">ArgentinaArgentinaArgentinaArgentinaArgentinaArgentina </option>
              <option value="Bolivia">Bolivia</option>
              <option value="Brazil">Brazil</option>
            </select>
          </div>
        </div>
      </div>
    </div>
  
    <div class="field is-horizontal">
      <div class="field-label">
        <label class="label">Select macros</label>
      </div>
      <div class="field-body">
        <div class="field">
          <div class="control">
            <div>
              <label class="checkbox">
                <input type="checkbox">
                AC power
              </label>
            </div>
            <div>
              <label class="checkbox">
                <input type="checkbox">
                DC power
              </label>
            </div>
          </div>
        </div>
      </div>
    </div>
  
    <div class="field is-horizontal">
      <div class="field-label">
        <!-- Left empty for spacing -->
      </div>
      <div class="field-body">
        <div class="field">
          <div class="control">
            <button class="button is-primary">
              Generate XML
            </button>
          </div>
        </div>
      </div>
    </div>
  </form>
</template>

<style scoped lang="scss"></style>
