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
                <h3 data-shadow="LINEN BLAZER">LINEN BLAZER</h3>
                <h4>01</h4>
                <h5>Men's outfit</h5>
                <div class="stripe"></div>
              </div>
            </div>
            </div>
          <div class="twoGroup half">
            <h4>02</h4>
            <div class="picGroup">
              <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[1]}')` }">
                <h3 data-shadow="FREELIFT">FREELIFT</h3>
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
                <h3 data-shadow="SUPER SKINNY">SUPER SKINNY</h3>
                <h4>03</h4>
                <h5>Men's pattern shirts</h5>
              </div>
            </div>
          </div>
          <div class="fiveGroup">
            <h3 data-shadow="SWEETSHIRTS">SWEETSHIRTS</h3>
            <div class="picGroup">
              <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[4]}')` }">
                <h4>05</h4>
                <h5>Men's jacket</h5>
                <div class="stripe"></div>
              </div>
            </div>
          </div>
        </div>
        <div class="fourGroup half">
          <div class="picGroup">
            <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[3]}')` }">
              <h3 data-shadow="DENIM">DENIM</h3>
              <h4>04</h4>
              <h5>Men's cadual</h5>
              <div class="stripe"></div>
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
              <h3 data-shadow="VINTAGE DENIM">VINTAGE DENIM</h3>
              <h4>06</h4>
              <h5>Men's classic</h5>
            </div>
          </div>
        </div>
        <div class="sevenGroup half">
          <div class="picGroup">
            <div class="pic fixGroup" :style="{ backgroundImage : `url('${picList[6]}')` }">
              <h3 data-shadow="EDITION">EDITION</h3>
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
    h4{
      font-size: 45px;
    }
    h3{
      font-size: 40px;
      position: relative;
      &:after{
        content: attr(data-shadow);
        position: absolute;
        left: 0;
        top: -20px;
        background: linear-gradient(rgba(0,0,0,0.1),transparent);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }
      &:before{
        content: attr(data-shadow);
        position: absolute;
        left: 0;
        top: -10px;
        background: linear-gradient(rgba(0,0,0,0.3),transparent);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }
    }
    .pic{
      background-size: cover;
      background-position: center;
      h5{
        font-size: 20px;
        font-style: italic;
      }
      &:before{
        position: absolute;
        content: '';
        border: 15px solid #50E3C2;
        box-sizing: border-box;
      }
      &:after{
        position: absolute;
        content: '';
        background-color: #50E3C2;
      }
    }
    .stripe{
      position: absolute;
      overflow: hidden;
      &:after{
        transform: rotate(30deg);
        top: -100% ;
        left: 10%;
        width: 20px;
        height: 200%;
        background-color: #50E3C2;
        box-shadow: 35px 0 0 #50E3C2,70px 0 0 #50E3C2,105px 0 0 #50E3C2,140px 0 0 #50E3C2,175px 0 0 #50E3C2;
        position: absolute;
        content: '';
      }
    }
    .oneTwoGroup{
      padding-top: 75%;
      .oneGroup{
        .picGroup{
          padding-top: 100%;
          .pic{
            h3{
              position: absolute;
              top: -20px;
            }
            h4{
              position: absolute;
              bottom: -10%;
            }
            h5{
              position: absolute;
              right: -14%;
              bottom: 7%;
              transform: rotate(90deg);
            }
            .stripe{
              bottom: -8%;
              left: 13%;
              width: 50%;
              height: 25%;
            }
            &:before{
              width: 50%;
              height: 50%;
              z-index: -1;
              right: -10%;
              top: -10%; 
            }
          }
        }
      }
      .twoGroup{
        position: relative;
        h4{
          position: absolute;
          right: 0;
          top: 0;
          z-index: 2;
          line-height: .8;
        }
        .picGroup{
          position: absolute;
          top: 20%;
          left: 50%;
          transform: translateX(-50%);
          width: 50%;
          padding-top: 50%;
          .pic{
            h3{
              position: absolute;
              right: -50%;
              bottom: -33%;
            }
            h5{
              position: absolute;
              left: -5%;
              top: -12%;
            }
            &:after{
              z-index: -1;
              width: 100%;
              height: 100%;
              right: -25%;
              top: -30%;
            }
            &:before{
              box-sizing: border-box;
              z-index: -1;
              width: 100%;
              height: 100%;
              right: -50%;
              top: -60%;
            }
          }
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
            .pic{
              h3{
                top: -20%;
                left: 0;
                position: absolute;
              }
              h5{
                position: absolute;
                bottom: -11%;
                left: 5%;
              }
              h4{
                position: absolute;
                right: -17%;
                bottom: -34%;
              }
              &:before{
                right: -17%;
                bottom: -30%;
                z-index: -1;
                width: 50%;
                height: 100%;
              }
            }
          }
        }
        .fiveGroup{
          display: flex;
          justify-content: flex-end;
          position: relative;
          h3{
            position: absolute;
            left: 0;
            top: 20%;
            z-index: 2;
          }
          .picGroup{
            width: 50%;
            padding-top: 50%;
            .pic{
              .stripe{
                width: 100%;
                height: 50%;
                left: -50%;
                top: -25%;
              }
              &:before{
                width: 100%;
                height: 50%;
                z-index: -1;
                left: -50%;
                bottom: -25%;
              }
              h4{
                left: -50%;
                bottom: 10%;
                position: absolute;
                line-height: 0.8;
              }
              h5{
                position: absolute;
                right: -50%;
                bottom: -10%;
              }
            }
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
          .pic{
            .stripe{
              width: 100%;
              height: 25%;
              bottom: -12%;
            }
            h3{
              position: absolute;
              left: -33%;
              top: 7%;
              transform: rotate(-90deg)
            }
            h4{
              position: absolute;
              left: -23%;
              bottom: 0;  
            }
            h5{
              position: absolute;
              transform: rotate(90deg);
              right: -3%;
              top: -15%;
            }
            &:before{
              z-index: -1;
              width: 100%;
              height: 50%;
              left: -34%;
              top: -20%;
            }
          }
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
          .pic{
            h3{
              position: absolute;
              top: -10%;
              right: 0;
            }
            h4{
              position: absolute;
              left: -12%;
              bottom: 50%;
            }
            h5{
              position: absolute;
              bottom: -5%;
              left: 50%;
              transform: translateX(-50%);
            }
            &:before{
              width: 100%;
              height: 25%;
              bottom: -10%;
              z-index: -1;
            }
            &:after{
              width: 50%;
              height: 50%;
              bottom: 0;
              left: -12%;
              z-index: -1;
            }
          }
        }
      }
      .sevenGroup{
        order: 0;
        padding-top: 25%;
        .picGroup{
          width: 50%;
          padding-top: 100%;
          .pic{
            h3{
              transform: rotate(90deg);
              position: absolute;
              right: -40%;
              top: 10%;
            }
            h4{
              position: absolute;
              left: 125%;
              bottom: 0;
              z-index: 2;
            }
            h5{
              position: absolute;
              bottom: 100%;
            }
            &:before{
              width: 100%;
              height: 100%;
              z-index: -1;
              position: absolute;
              left: 25%;
              top: -10%;
            }
            &:after{
              width: 50%;
              height: 50%;
              left: 100%;
              bottom: 0;
            }
          }
        }
      }
    }
  }
</style>
