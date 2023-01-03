<template>
  <div class="container">
    <div class="sendInfo">
      <div class="one">보내는사람</div>
      <div class="two">받는사람</div>
      <div class="three">제목</div>
      <div class="four">첨부파일</div>
      <div class="five">끌어오기</div>
      <div class="one2">
        <input type="text" class="input" /><button>계정</button>
      </div>
      <div class="two2">
        <input type="text" class="input" /><button>주소록</button>
      </div>
      <div class="three2"><input type="text" class="input" /></div>
      <div class="four2"><button>내 PC</button></div>
      <div class="five2"><div>마우스로 끌어오기</div></div>
    </div>
    <div class="six">
      <textarea
        class="mail"
        name="mail"
        id="mail"
        cols="155px"
        rows="20px"
      ></textarea>
    </div>
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
  /* border-style: solid; */
 }
.two {
   grid-area: two;
   /* background-color: lightgoldenrodyellow; */
   /* border-style: solid; */
   }
.three { 
  grid-area: three;
  /* background-color: lightcoral; */
  /* border-style: solid; */
 }
.four {
   grid-area: four; 
   /* background-color: lightgoldenrodyellow; */
   /* border-style: solid; */
  }
.five {
   grid-area: five; 
   /* background-color: lightcoral; */
   /* border-style: solid; */
  }
.six { 
  grid-area: six; 
  /* background-color: lightgoldenrodyellow; */
  /* border-style: solid; */
}
.seven {
   grid-area: seven;
   /* background-color: lightcoral; */
   /* border-style: solid; */
   }
.one2{
  grid-area: one2;
  background-color: lightblue;
  /* border-style: solid; */
}
.two2{
  grid-area: two2;
  /* background-color: lightblue; */
  /* border-style: solid; */
}
.three2{
  grid-area: three2;
  /* background-color: lightblue; */
  /* border-style: solid; */
}
.four2{
  grid-area: four2;
  /* background-color: lightblue; */
  /* border-style: solid; */
}
.five2{
  grid-area: five2;
  /* background-color: lightblue; */
  /* border-style: solid; */
}
.mail{
  margin: 1% 1% 1% 1%;
  resize:none;/* 크기고정 */ 
  overflow: auto;
}
.input{
  width: 800px;
}
</style>
