<template>
  <div class="content">
  <md-card>
    <md-card-header data-background-color="green">
      <h4 class="title">拖轮状态</h4>
    </md-card-header>

    <md-card-content>
      <div class="md-layout">
        <div class="md-layout-item md-medium-size-50 md-xsmall-size-100 md-size-33">
          <status-list :index.sync="index" :data="data"></status-list>
        </div>
        <div class="md-layout-item md-medium-size-50 md-xsmall-size-100 md-size-66">
          <status-map :index="index" :info="data"></status-map>
        </div>
      </div>
    </md-card-content>
  </md-card>
  </div>
</template>

<script>
import StatusList from "@/pages/Task/StatusList.vue"
import StatusMap from "@/pages/Task/StatusMap.vue"

export default {
  components: {
    StatusList,
    StatusMap
  },
  data() {
    return {
      index: 0,
      data: [
        {
          title: "Nanhai228 锚9至码头5（港拖15）",
          path: [
            [122.030967,31.370827],
            [122.03497831,31.36166679],
            [122.03898962,31.35250659],
            [122.04300093,31.34334638],
            [122.04701224,31.33418617],
            [122.05102355,31.32502597],
            [122.05503487,31.31586576],
            [122.05871009,31.30673209],
            [122.06171314,31.29765149],
            [122.06404401,31.28862396],
            [122.06570271,31.27964951],
            [122.06668924,31.27072812],
            [122.06700359,31.26185981],
            [122.06664576,31.25304457],
            [122.06561576,31.2442824 ],
            [122.06353387,31.23563539],
            [122.06073271,31.2271094 ],
            [122.05727254,31.21869967],
            [122.05321363,31.21040143],
            [122.04861623,31.20220994],
            [122.04354061,31.19412042],
            [122.03804703,31.18612814],
            [122.03219574,31.17822832],
            [122.02604701,31.17041621],
            [122.0196611, 31.16268705],
            [122.01297716,31.15522414],
            [122.00605364,31.14813406],
            [121.99889447,31.14141187],
            [121.99150359,31.1350526 ],
            [121.98388495,31.12905133],
            [121.97604247,31.1234031 ],
            [121.96798009,31.11810297],
            [121.95970176,31.113146],
            [121.95111258,31.10868567],
            [121.9423378, 31.10452279],
            [121.93339551,31.10062817],
            [121.92430381,31.09697263],
            [121.91508081,31.093527],
            [121.90574459,31.09026209],
            [121.89631326,31.08714873],
            [121.88680491,31.08415775],
            [121.87723765,31.08125995],
            [121.86762956,31.07842618],
            [121.85799875,31.07562724],
            [121.84836331,31.07283396],
            [121.83874135,31.07001716],
            [121.82915095,31.06714766],
            [121.81958238,31.0642421 ]
          ],
          status: "run"
        },
        {
          title: "NanFang 锚10至码头3（港拖16）",
          path: [
            [122.036716,31.271125],
            [122.03134398,31.26269046],
            [122.02597196,31.25425593],
            [122.02048964,31.24595663],
            [122.01478675,31.23792779],
            [122.00886327,31.23016941],
            [122.00271921,31.2226815 ],
            [121.99635457,31.21546406],
            [121.98976934,31.20851708],
            [121.98296354,31.20184056],
            [121.97593715,31.19543451],
            [121.96869018,31.18929892],
            [121.96122262,31.1834338 ],
            [121.95341798,31.17798302],
            [121.94539108,31.17280683],
            [121.93715803,31.16788548],
            [121.92873495,31.16319921],
            [121.92013793,31.15872826],
            [121.91138311,31.15445288],
            [121.90248658,31.15035331],
            [121.89346447,31.14640979],
            [121.88433289,31.14260257],
            [121.87510794,31.1389119 ],
            [121.86580574,31.13531801],
            [121.8564424, 31.13180115],
            [121.84703404,31.12834157],
            [121.83759677,31.1249195 ],
            [121.8281467, 31.1215152 ],
            [121.81869994,31.1181089 ],
            [121.80927261,31.11468085],
            [121.79988081,31.11121129],
            [121.79051215,31.1077144 ]
          ],
          status: "run"
        },
        {
          title: "CCST20 锚20至码头1（港拖13）",
          path: [
            [122.040166,31.270137],
            [122.03945825,31.26016208],
            [122.03854898,31.25026752],
            [122.03723666,31.24053368],
            [122.03552129,31.23096058],
            [122.03340287,31.2215482 ],
            [122.0308814, 31.21229654],
            [122.02795687,31.20320561],
            [122.0246293, 31.19427541],
            [122.02089868,31.18550594],
            [122.0164837, 31.17710393],
            [122.01152658,31.16910724],
            [122.00605802,31.16150363],
            [122.00010872,31.15428085],
            [121.99370938,31.14742667],
            [121.9868907, 31.14092883],
            [121.97968339,31.13477509],
            [121.97211814,31.12895322],
            [121.96422566,31.12345097],
            [121.95603664,31.1182561 ],
            [121.9474915, 31.11349033],
            [121.93877693,31.10897675],
            [121.92990968,31.10469173],
            [121.92090648,31.10061164],
            [121.91178408,31.09671285],
            [121.9025592, 31.09297173],
            [121.89324859,31.08936465],
            [121.88386899,31.08586798],
            [121.87443714,31.08245809],
            [121.86496976,31.07911135],
            [121.85548361,31.07580413],
            [121.84599542,31.0725128 ],
            [121.83652193,31.06921372],
            [121.82707988,31.06588328],
            [121.81765912,31.06252927]
          ],
          status: "stop"
        },
        {
          title: "TEXAS TRADER 码头4至锚地3",
          path: [
            [122.098807,31.181203],
            [122.10134141,31.17152949],
            [122.10344347,31.1620005 ],
            [122.10468083,31.15276053],
            [122.1050535, 31.14380959],
            [122.10456147,31.13514769],
            [122.10320475,31.12677481],
            [122.10098333,31.11869096],
            [122.09789722,31.11089614],
            [122.09394641,31.10339035],
            [122.08913091,31.09617358],
            [122.08345071,31.08924585],
            [122.07690582,31.08260715],
            [122.06949623,31.07625747],
            [122.06165429,31.07005231],
            [122.05373501,31.06400411],
            [122.04566103,31.05826984],
            [122.03743236,31.0528495 ],
            [122.029049,31.04774308],
            [122.02051095,31.04295059],
            [122.0118182, 31.03847203],
            [122.00297077,31.0343074 ],
            [121.99389806,31.03059541],
            [121.98469459,31.0271398 ],
            [121.97537593,31.02390896],
            [121.96595765,31.02087126],
            [121.95645534,31.01799511],
            [121.94688457,31.01524889],
            [121.93726092,31.01260099],
            [121.92759995,31.01001981],
            [121.91791726,31.00747372],
            [121.90822842,31.00493111],
            [121.898549,31.00236039],
            [121.88889458,30.99972993],
            [121.87925785,30.99705908],
            [121.86962113,30.99438822]
          ],
          status: "run"
        },
        {
          title: "SummerEast 码头6至锚地5",
          path: [
            [121.903336,31.346158],
            [121.91064109,31.33932897],
            [121.91786305,31.33243141],
            [121.92491873,31.32539678],
            [121.93180812,31.31822508],
            [121.93853124,31.3109163 ],
            [121.94508808,31.30347046],
            [121.95147864,31.29588754],
            [121.95770292,31.28816756],
            [121.96349351,31.2802228 ],
            [121.96875565,31.27210789],
            [121.97349892,31.26383074],
            [121.97773291,31.25539924],
            [121.9814672, 31.24682129],
            [121.98471135,31.23810478],
            [121.98747496,31.22925762],
            [121.98976761,31.22028769],
            [121.99159887,31.21120291],
            [121.99297832,31.20201115],
            [121.99391554,31.19272033],
            [121.99404631,31.18340232],
            [121.99345119,31.17421593],
            [121.99216278,31.16516665],
            [121.99021369,31.15625996],
            [121.98763652,31.14750136],
            [121.98446387,31.13889634],
            [121.98072835,31.13045037],
            [121.97646255,31.12216894],
            [121.97169907,31.11405754],
            [121.96628945,31.10621755],
            [121.96053751,31.09855901],
            [121.95447307,31.09106651],
            [121.94812592,31.08372462],
            [121.94152584,31.07651789],
            [121.93470265,31.0694309 ],
            [121.92768613,31.06244822],
            [121.92050609,31.05555441],
            [121.91319231,31.04873404],
            [121.90577459,31.04197168],
            [121.89828274,31.03525189],
            [121.89074654,31.02855925],
            [121.88319579,31.02187833],
            [121.87566029,31.01519368],
            [121.86816983,31.00848988],
            [121.86075421,31.0017515 ],
            [121.85338595,30.99499068],
            [121.84601768,30.98822987]
          ],
          status: "wait"
        },
        {
          title: "GreatWall 码头7至锚地1",
          path: [
            [122.05871009,31.30673209],
            [122.06171314,31.29765149],
            [122.06404401,31.28862396],
            [122.06570271,31.27964951],
            [122.06668924,31.27072812],
            [122.06700359,31.26185981],
            [122.06664576,31.25304457],
            [122.06561576,31.2442824 ],
            [122.06353387,31.23563539],
            [122.06073271,31.2271094 ],
            [122.05727254,31.21869967],
            [122.05321363,31.21040143],
            [122.04861623,31.20220994],
            [122.04354061,31.19412042],
            [122.03804703,31.18612814],
            [122.03219574,31.17822832],
            [122.02604701,31.17041621],
            [122.0196611, 31.16268705],
            [122.01297716,31.15522414],
            [122.00605364,31.14813406],
            [121.99889447,31.14141187],
            [121.99150359,31.1350526 ],
            [121.98388495,31.12905133],
            [121.97604247,31.1234031 ],
            [121.96798009,31.11810297],
            [121.95970176,31.113146],
            [121.95111258,31.10868567],
            [121.9423378, 31.10452279],
            [121.93339551,31.10062817],
            [121.92430381,31.09697263],
            [121.91508081,31.093527],
            [121.90574459,31.09026209],
            [121.89631326,31.08714873],
            [121.88680491,31.08415775],
            [121.87723765,31.08125995],
            [121.86762956,31.07842618],
            [121.85799875,31.07562724],
            [121.84836331,31.07283396],
            [121.83874135,31.07001716],
            [121.82915095,31.06714766],
            [121.81958238,31.0642421 ]
          ],
          status: "wait"
        }
      ],
      pos: {
        lng: 122.22001,
        lat: 31.154579
      },
      center: {
        lng: 121.845001,
        lat: 31.154579
      }
    }
  },
}
</script>
