<template>
  <div class="content">
    <div class="row layout">
      <div class="col slogan">
        <span class="yellow">Sweet deals</span><br/>
        <span class="yellow">in crypto</span><br/>
        <span class="yellow">mining.</span><br/>
        <span class="black">BEST PRICE  x  OBJECTIVE METRICS</span>
      </div>
      <div class="col">
        <div class="desc">We aggregate and rate existing cloud mining contracts, for transparency, standardization and price discovery.</div>
        <div class="desc sign_up">Sign up for fresh updates & never miss a juicy deal.</div>

        <div class="row form">
          <label for="email" style="display: none;">email</label>
          <input id="email" type="email" placeholder="Enter email address" />
          <a class="btn">GO</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.content {
  padding-bottom: 100px;
  margin: 120px 70px 0 70px;

  .row {
    display: flex;
    flex-wrap: wrap;
  }

  .row.layout {
    /*max-width: 1100px;*/
    justify-content: space-around;
    align-items: flex-start;

    .slogan {
      /*width: 480px;*/
      > span {
        display: inline-block;

        &.yellow {
          background-color: #fef807;
          padding: 5px 10px;
          font-size: 44px;
          margin: 10px 0;
          box-shadow: 5px 5px 5px #888888;
          text-shadow: 2px 2px 2px #888888;
        }

        &.black {
          background-color: black;
          color: #fef807;
          margin-top: 50px;
          padding: 2px 5px;
          font-size: 18px;
        }
      }
    }

    .desc {
      margin: 10px 0 10px 0;
      font-size: 20px;
      max-width: 527px;

      &.sign_up {
        margin: 160px 0 20px 0;
      }
    }
  }

  .row.form {
    align-items: center;

    input {
      font-family: 'Eras ITC', 'Avenir', Helvetica, Arial, sans-serif;
      font-size: 20px;
      padding: 10px;
      margin-right: 10px;
      border: 1px solid black;
      border-radius: 5px;
      box-shadow: 3px 3px 3px #888888;
      flex-grow: 1;

      &::placeholder {
        font-size: 20px;
      }
    }

    .btn {
      cursor: pointer;
      background-image: url("../assets/logo.png");
      background-size: 80px;
      width: 80px;
      height: 62px;
      text-align: center;
      line-height: 62px;
      font-size: 20px;
    }
  }
}

@media screen and (max-width: 980px) {
  .content {
    margin: 60px 15px 0 15px;

    .row.layout {
      .black {
        margin-top: 10px!important;
      }

      .desc.sign_up {
        margin: 20px 0;
      }
    }
  }
}
</style>
