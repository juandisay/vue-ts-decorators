# vue typescript snippets

Code snippets for vue component and vuex store with typescript

### Usage

 Type part of a snippet, press `Enter` or `Tab`, and the snippet unfolds. 

#### Snippets

##### .vue files snippets

+ v - init  

  ```vue
  <template>
    <div>
      
    </div>
  </template>
  <script lang='ts'>
  import { Component, Prop, Vue } from 'vue-property-decorator'
  
  @Component({
    name: '',
    components:{
      
    }
  })
  export default class ComponentName extends Vue {
    
  }
  </script>
  
  <style lang='scss' scoped>
    
  </style>
  ```

  

##### Vuex store module snippets

+ vx - init  

  ```typescript
  import Vue from 'vue'
  import Vuex from 'vuex'
  
  Vue.use(Vuex)
  
  export interface IRootState{
    
  }
  
  export default new Vuex.Store<IRootState>({})
  ```

  

+ vx - module

  ```typescript
  import { VuexModule, Module, getModule, Action, Mutation } from 'vuex-module-decorators'
  import store from '@/store/index'
  
  export interface IModuleState{
    
  }
  
  @Module({ name: 'name', store, dynamic: true })
  class ModuleName extends VuexModule implements IModuleState {
    
  }
  
  export const ModuleNameModule = getModule(ModuleName)
  ```

  

