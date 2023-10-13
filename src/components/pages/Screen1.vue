<template>
  <DropZone ncBgType="bgColor" backgroundImage="" id="0e0fc853-006b-47fb-895e-fe21bd833617"
    v-bind:style="{'width':'100%','height':'auto'}">
    <AdvanceDatatable v-bind:items="bindSource('functions.breeds.data.data')"
      v-bind:fields="[{'label':'Breed','key':'breed','sortable':true,'searchable':true,'class':''},{'label':'Country','key':'country','sortable':true,'searchable':true,'class':''},{'label':'Origin','key':'origin','sortable':true,'searchable':true,'class':''},{'label':'Coat','key':'coat','sortable':true,'searchable':true,'class':''},{'label':'Pattern','key':'pattern','sortable':true,'searchable':true,'class':''}]"
      v-bind:isBusy="false" v-bind:isFixed="true" v-bind:isHover="false" mapping="functions.breeds.data.data"
      v-bind:perPage="5" emptyTxt="This datatable is currently empty, but you can customize it with your information."
      v-bind:isStriped="true" hoverColor="#EDEDED" selectMode="multi" v-bind:allowExport="true" borderColor="#cdcdcd"
      emptyHeader="Header" v-bind:isFootClone="false" v-bind:outerBorder="true" downloadType="CSV"
      v-bind:isResponsive="true" v-bind:isSelectable="true" v-bind:hasPagination="true" v-bind:searchControl="true"
      v-bind:showTotalRows="true"
      emptyFilterTxt="Please consider using different keywords or filters and try your search again."
      v-bind:filterDebounce="0" v-bind:smallSelection="false" textDecoration="none" headerTextColor="#606060"
      v-bind:isFooterSorting="true" selectedRowColor="#E3EEFB" borderAffectedArea="all" v-bind:defaultSelectedRow="0"
      v-bind:refreshButtonControl="true" v-bind:tableBodyOuterBorder="true" headerBackgroundColor="#FFFFFF"
      cellVerticalBorderColor="#cdcdcd" v-bind:tableCellVerticalBorder="true" cellHorizontalBorderColor="#cdcdcd"
      tableBodyOuterBorderColor="#cdcdcd" v-bind:tableCellHorizontalBorder="true" position="relative"
      v-bind:snapX="false" v-bind:snapY="false" id="6107b924-474c-4cd9-993d-5b57ff964269"
      v-bind:style="{'color':'#606060','width':'100%','height':'100%','minWidth':'350px','fontStyle':'normal','minHeight':'150px','textAlign':'left','wordBreak':'keep-all','background':'#FFFFFF','fontFamily':'Inter','fontWeight':400,'textIndent':'0px','visibility':'visible','whiteSpace':'nowrap','wordSpacing':'0px','letterSpacing':'0px','textTransform':'none','zIndex':2}"/>
  </DropZone>
</template>
<script>
import { mapGetters } from 'vuex';
export default {
  name: 'Screen1',
  data() {
    return {};
  },
  props: {},
  created() {},
  mounted() {},
  computed: { ...mapGetters('source', ['getApiMappingWithChain'])},
  methods: {bindSource(chain) { return this.getApiMappingWithChain(chain); }},
  watch: {},
};
</script>

<style lang="scss" scoped>@media (min-width: 1024.05px){
[id='0e0fc853-006b-47fb-895e-fe21bd833617'] {
             display: grid; 
             grid-template-columns: 13.125rem 51.640625rem 35.234375rem;
             grid-template-rows: minmax(8.828125rem, max-content) minmax(29.375rem, max-content) minmax(16.71875rem, max-content);
          }
[id='6107b924-474c-4cd9-993d-5b57ff964269']{
          grid-area: 2/2/3/3;
          font-size: Max(Min(14rem, 12px),1.09375rem);
          }
}
@media (min-width: 768.05px) and (max-width: 1024px){
[id='0e0fc853-006b-47fb-895e-fe21bd833617'] {
             display: grid; 
             grid-template-columns: 17.724609375rem 64.55078125rem 17.724609375rem;
             grid-template-rows: minmax(11.03515625rem, max-content) minmax(36.71875rem, max-content) minmax(3.125rem, max-content);
          }
[id='6107b924-474c-4cd9-993d-5b57ff964269']{
          grid-area: 2/2/3/3;
          font-size: Max(Min(14rem, 12px),1.3671875rem);
          }
}
@media (min-width: 480.05px) and (max-width: 768px){
[id='0e0fc853-006b-47fb-895e-fe21bd833617'] {
             display: grid; 
             grid-template-columns: 4.166666667000001rem 91.666666666rem 4.166666667000001rem;
             grid-template-rows: minmax(14.713541666666666rem, max-content) minmax(52.143217347074135rem, max-content) minmax(4.166666667rem, max-content);
          }
[id='6107b924-474c-4cd9-993d-5b57ff964269']{
          grid-area: 2/2/3/3;
          font-size: Max(Min(14rem, 12px),1.9415027735612709rem);
          }
}
@media (min-width: 375.05px) and (max-width: 480px){
[id='0e0fc853-006b-47fb-895e-fe21bd833617'] {
             display: grid; 
             grid-template-columns: 5rem 90rem 5rem;
             grid-template-rows: minmax(23.541666666666668rem, max-content) minmax(51.195158850226925rem, max-content) minmax(5rem, max-content);
          }
[id='6107b924-474c-4cd9-993d-5b57ff964269']{
          grid-area: 2/2/3/3;
          font-size: Max(Min(14rem, 12px),1.906202723146747rem);
          }
}
@media (min-width: 0px) and (max-width: 375px){
[id='0e0fc853-006b-47fb-895e-fe21bd833617'] {
             display: grid; 
             grid-template-columns: 6.4rem 87.2rem 6.4rem;
             grid-template-rows: minmax(30.133333333333333rem, max-content) minmax(49.60242057488654rem, max-content) minmax(6.4rem, max-content);
          }
[id='6107b924-474c-4cd9-993d-5b57ff964269']{
          grid-area: 2/2/3/3;
          font-size: Max(Min(14rem, 12px),1.8468986384266264rem);
          }
}
</style>