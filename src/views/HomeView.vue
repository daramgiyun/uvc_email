<template>
  <div class="container">
    <div class="sendInfo">
      <div class="one">보내는사람</div>
      <div class="two">받는사람</div>
      <div class="three">제목</div>
      <div class="four">첨부파일</div>
      <div class="five">끌어오기</div>
      <div class="one2">2</div>
      <div class="two2">2</div>
      <div class="three2">2</div>
      <div class="four2">2</div>
      <div class="five2">2</div>
    </div>
    <div class="six">내용</div>
    <div class="seven">
      <button>취소</button>
      <button>전송</button>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.container {
  display: grid; 
  grid-template-columns: 100%; 
  grid-template-rows: 270px 530px 100px; 
  gap: 0px 0px; 
  grid-template-areas: 
    "sendInfo"
    "six"
    "seven"; 
  margin-top: 1%;
  /* text-align: center; */
  /* align-items: center; */
  background-color: lightcyan;
}
.sendInfo {
  display: grid; 
  grid-template-columns: 30% 70%; 
  grid-template-rows: 50px 50px 50px 50px 70px; 
  gap: 0px 0px; 
  grid-template-areas: 
    "one one2"
    "two two2"
    "three three2"
    "four four2"
    "five five2"; 
  grid-area: sendInfo; 
  text-align: center;
  align-items: center;
  background-color: lightseagreen ;
}
.one { 
  grid-area: one;
  /* background-color: lightcoral; */
  border-style: solid;
 }
.two {
   grid-area: two;
   /* background-color: lightgoldenrodyellow; */
   border-style: solid;
   }
.three { 
  grid-area: three;
  /* background-color: lightcoral; */
  border-style: solid;
 }
.four {
   grid-area: four; 
   /* background-color: lightgoldenrodyellow; */
   border-style: solid;
  }
.five {
   grid-area: five; 
   /* background-color: lightcoral; */
   border-style: solid;
  }
.six { 
  grid-area: six; 
  background-color: lightgoldenrodyellow;
  border-style: solid;
}
.seven {
   grid-area: seven;
   /* background-color: lightcoral; */
   border-style: solid;
   }
.one2{
  grid-area: one2;
  /* background-color: lightblue; */
  border-style: solid;
}
.two2{
  grid-area: two2;
  /* background-color: lightblue; */
  border-style: solid;
}
.three2{
  grid-area: three2;
  /* background-color: lightblue; */
  border-style: solid;
}
.four2{
  grid-area: four2;
  /* background-color: lightblue; */
  border-style: solid;
}
.five2{
  grid-area: five2;
  /* background-color: lightblue; */
  border-style: solid;
}
</style>
