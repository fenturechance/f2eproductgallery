<template>
  <div id="app">
    <header class="group">
      <div class="fixGroup">
        <h2 class="smallTag">CCCLOTHES</h2>
        <h1>MEN'S TOPS</h1>
      </div>
    </header>
    <div class="oneTwoGroup group">
        <div class="fixGroup">
          <div class="oneGroup half">
            <div class="picGroup">
              <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[0]}')` }">
                <h3>LINEN BLAZER</h3>
                <h4>01</h4>
                <h5>Men's outfit</h5>
                <div class="stripe"></div>
              </div>
            </div>
            </div>
          <div class="twoGroup half">
            <div class="picGroup">
              <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[1]}')` }">
                <h3>FREELIFT</h3>
                <h4>02</h4>
                <h5>Men's basics</h5>
              </div>
            </div>
          </div>
        </div>
    </div>
    <div class="threeFourFiveGroup group">
      <div class="fixGroup">
        <div class="threeFiveGroup half">
          <div class="threeGroup">
            <div class="picGroup">
              <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[2]}')` }">
                <h3>SUPER SKINNY</h3>
                <h4>03</h4>
                <h5>Men's pattern shirts</h5>
              </div>
            </div>
          </div>
          <div class="fiveGroup">
            <div class="picGroup">
              <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[4]}')` }">
                <h3>SWEETSHIRTS</h3>
                <h4>05</h4>
                <h5>Men's jacket</h5>
              </div>
            </div>
          </div>
        </div>
        <div class="fourGroup half">
          <div class="picGroup">
            <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[3]}')` }">
              <h3>DENIM</h3>
              <h4>04</h4>
              <h5>Men's cadual</h5>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="sixSevenGroup group">
      <div class="fixGroup">
        <div class="sixGroup half">
          <div class="picGroup">
            <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[5]}')` }">
              <h3>VINTAGE DENIM</h3>
              <h4>06</h4>
              <h5>Men's classic</h5>
            </div>
          </div>
        </div>
        <div class="sevenGroup half">
          <div class="picGroup">
            <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[6]}')` }">
              <h3>EDITION</h3>
              <h4>07</h4>
              <h5>Men's shirts</h5>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      picList : [
        'https://images.unsplash.com/photo-1513827379601-9dba5099a3f9?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=1acdd78f34ee75aade9e313251bb1695&auto=format&fit=crop&w=334&q=80',
        'https://images.unsplash.com/photo-1514632542677-48fae74a01b2?ixlib=rb-0.3.5&s=50945fdb784e64361154c62785542531&auto=format&fit=crop&w=334&q=80',
        'https://images.unsplash.com/photo-1496345875659-11f7dd282d1d?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=a0f994eef47e5fb1a67849703cc961b3&auto=format&fit=crop&w=1050&q=80',
        'https://images.unsplash.com/photo-1484516758160-69878111a911?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=39466d66952b133d5a5cff642b970d05&auto=format&fit=crop&w=387&q=80',
        'https://images.unsplash.com/photo-1525448198276-222de3961638?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=43fb25556cdbd191e520c7f28739e40d&auto=format&fit=crop&w=1050&q=80',
        'https://images.unsplash.com/photo-1519406709381-c1f293304b28?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=98c497a29f229085d9574ee8b6eeef8c&auto=format&fit=crop&w=334&q=80',
        'https://images.unsplash.com/photo-1516914943479-89db7d9ae7f2?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=63ff45d79414b3166b08b800a32018be&auto=format&fit=crop&w=334&q=80'
      ]
    }
  }
}
</script>

<style lang="scss">
  *{
    padding: 0;
    margin: 0;
    font-family: 'Roboto', sans-serif;
  }
  div{
    box-sizing: border-box;
  }
  #app{
    padding: 20px;
    max-width: 986px;
    margin: auto;
    .group{
      position: relative;
    }
    .fixGroup{
      position: absolute;
      display: flex;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
    }
    .half{
      flex: 5;
    }
    header{
      text-align: center;
      padding-top: 25%;
      .fixGroup{
        display: block;
      }
      .smallTag{
        background-color: #000;
        color: #fff;
        display: inline-block;
        padding: 2px 10px;
        font-size: 18px;
        margin: 5px 0;
      }
      h1{
        font-weight: bold;
        font-size: 60px;
      }
    }
    .picGroup{
      position: relative;
    }
    .pic{
      background-size: cover;
      background-position: center;
    }
    .oneTwoGroup{
      padding-top: 75%;
      .oneGroup{
        .picGroup{
          padding-top: 100%;
          .pic{
            
          }
        }
      }
      .twoGroup{
        position: relative;
        .picGroup{
          position: absolute;
          top: 20%;
          left: 50%;
          transform: translateX(-50%);
          width: 50%;
          padding-top: 50%;
        }
      }
    }
    .threeFourFiveGroup{
      padding-top: 87.5%;
      .threeFiveGroup{
        .threeGroup{
          padding: 25% 0 50% 0;
          .picGroup{
            padding-top: 50%;
          }
        }
        .fiveGroup{
          display: flex;
          justify-content: flex-end;
          .picGroup{
            width: 50%;
            padding-top: 50%;
          }
        }
      }
      .fourGroup{
        padding: 12.5% 0 0 0;
        position: relative;
        .picGroup{
          right: 0;
          position: absolute;
          width: 50%;
          padding-top: 100%;
        }
      }
    }
    .sixSevenGroup{
      padding-top: 75%;
      .sixGroup{
        order: 1;
        .picGroup{
          width: 100%;
          padding-top: 100%;
        }
      }
      .sevenGroup{
        order: 0;
        padding-top: 25%;
        .picGroup{
          width: 50%;
          padding-top: 100%;
        }
      }
    }
  }
</style>
