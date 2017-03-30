<template >
  <div class="list">
      <div class="list-item" v-for="(item,index) in words">
        <div class="list-item-top">
            <span class="words">{{ item.word }}</span>
            <a :href="'http://dict.youdao.com/dictvoice?audio='+item.word+'&type=1'" class="play"></a>
        </div>
        <div class="pronunciation">
            <span class="right">✅： {{ item.right }}</span>
            <span class="wrong">❌： {{ item.wrong }}</span>
        </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'list',
  data () {
    return {
      words: [
          {
            word: 'access',
            right: "['ækses]",
            wrong: "[ək'ses]"
          },
          {
            word: 'analogy',
            right: "[əˈnælədʒi]",
            wrong: "[ænə'lɒdʒi]"
          },
          {
            word: 'Angular',
            right: "['æŋgjʊlə]",
            wrong: "['æŋɡələ]"
          },
          {
            word: 'AJAX',
            right: "['eidʒæks]",
            wrong: "[ə'dʒʌks]"},
          {
            word: 'Apache',
            right: "[ə'pætʃɪ]",
            wrong: "[ʌpʌtʃ]"
            },
          {
              word: 'app',
            right: "[æp]",
            wrong: "[eipi'pi]"
          },
          {
              word: 'archive',
              right: "['ɑːkaɪv]",
              wrong: "['ətʃɪv]"
          },
          {
              word: 'array',
              right: "[ə'rei]",
              wrong: "[æ'rei]"
        }
            ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
  font-size: 1.5rem;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  display: inline-flex;
}
.list-item-top{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.list-item{
    padding: 10px 20px;
    border-bottom: 1px solid #ddd;
}
.words{
    font-size: 1.5rem;
}
.play{
  width: 2rem;
  height: 2rem;
  background: url("../assets/play.png") no-repeat center;
  background-size: 100% 100%;
}
.pronunciation{
    display: flex;
    justify-content: space-between;
}
.right{
    padding-right: 2rem;
}
.wrong{
    text-decoration: line-through;
}
</style>
