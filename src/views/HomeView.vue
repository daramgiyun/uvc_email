<template>
  <div class="container">
    <div class="a">
      <div class="one">보내는 사람</div>
      <div class="two">받는 사람</div>
      <div class="three">제목</div>
      <div class="four">첨부 파일</div>
    </div>
    <div class="b">
      <div class="one2">
        <input class="input" type="text" /><button>계정</button>
      </div>
      <div class="two2">
        <input class="input" type="text" /><button>주소록</button>
      </div>
      <div class="three2"><input class="input" type="text" /></div>
      <div class="four2"><button>내 PC</button></div>
      <div class="four3">끌어오기</div>
    </div>
    <div class="six">
      <textarea
        class="mail"
        name="mail"
        id="mail"
        cols="155px"
        rows="22px"
      ></textarea>
    </div>
    <div class="seven">
      <button>취소</button>
      <button>보내기</button>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.container {  display: grid;
  grid-template-columns: 20% 80%;
  grid-template-rows: 270px 560px 70px;
  gap: 0px 0px;
  grid-auto-flow: row;
  grid-template-areas:
    "a b"
    "six six"
    "seven seven";
  background-color: lightcyan;
  margin-top: 2%;
}

.a {  display: grid;
  grid-template-rows: 55px 55px 55px 105px;
  gap: 0px 0px;
  grid-auto-flow: row;
  grid-area: a;
  background-color: lightseagreen;
  text-align: center;
  align-items: center;
}

.one {
  grid-area: 1 / 1 / 2 / 2;
  background-color: lightcoral;
 }

.two {
   grid-area: 2 / 1 / 3 / 2; 
   background-color: lightgoldenrodyellow;
   }

.three {
   grid-area: 3 / 1 / 4 / 2; 
    background-color: lightcoral;

   }

.four {
   grid-area: 4 / 1 / 5 / 2; 
   background-color: lightgoldenrodyellow;
   }

.b {
  display: grid;
  grid-template-rows: 55px 55px 55px 30px 75px;
  grid-auto-columns: 1fr;
  gap: 0px 0px;
  grid-auto-flow: row;
  grid-area: b;
  background-color: lightgreen;
  /* text-align: center; */
  /* align-items: center; */
}

.one2 { 
  grid-area: 1 / 1 / 2 / 2;
  background-color: lightgoldenrodyellow;
  display: block;
  align-self: center;
  display: flex;
  }

.two2 { 
  grid-area: 2 / 1 / 3 / 2; 
  background-color: lightcoral;
  display: block;
  align-self: center;
  display: flex;
}

.three2 {
  grid-area: 3 / 1 / 4 / 2; 
  background-color: lightgoldenrodyellow;
  display: block;
  align-self: center;
  display: flex;
  }

.four2 { 
  grid-area: 4 / 1 / 5 / 2;
  background-color: lightcoral;
  display: block;
  align-self: center;
 }

.four3 {
   grid-area: 5 / 1 / 6 / 2;
   background-color: lightcoral;
   }

.six { grid-area: six; 
background-color: lightslategray;}

.seven {
  grid-area: seven; 
  background-color: lightgoldenrodyellow;
  display: block;
  align-self: center;
  display: flex;
  justify-content: flex-end;
  }

.input {
  width: 900px;
}

.mail{
  margin: 1% 1% 1% 1%;
  resize:none;/* 크기고정 */ 
  overflow: auto;
}


</style>
