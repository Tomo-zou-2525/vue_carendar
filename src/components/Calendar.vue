<template>
  <div>
    <h1>カレンダーサンプル</h1>
  </div>
</template>

<script>
export default {
  data() {
    //暫定で3月の日付を指定
    return {
      weekdays: ["日", "月", "火", "水", "木", "金", "土"],
      year: 2020,
      month: 3,
      day: -1,
      today: ""
    };
  },
  computed: {
    // １週間の日付を呼び出す算術プロパティ
    calData: function() {
      console.log(this.year + "-" + this.month + "のデータ作成");
      var calData = [];

      calData[0] = [1, 2, 3, 4, 5, 6, 7];
      calData[1] = [8, 9, 10, 11, 12, 13, 14];
      calData[2] = [15, 16, 17, 18, 19, 20, 21];
      calData[3] = [22, 23, 24, 25, 26, 27, 28];
      calData[4] = [29, 30, 31, "", "", "", ""];

      return calData;
    }
  }
};
</script>
