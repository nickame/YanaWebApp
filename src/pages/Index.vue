<template>
  <q-page class="flex flex-center">
  <div class = "container">
    <section id="main" class="main">
      <q-img
       src="../assets/main-picture-gray.jpg"
       class="avatar"
       spinner-color="white"
       style="height: 300px; max-width: 800px"
      />
      <q-btn color="secondary" label="напиши мне напиши" />
    </section>
    <section id="abaut">
      <h2>пару слов о себе</h2>
      <p>Безусловно, курс на социально-ориентированный национальный проект играет определяющее значение для системы обучения кадров, соответствующей насущным потребностям. Значимость этих проблем настолько очевидна, что укрепление и развитие внутренней структуры прекрасно подходит для реализации дальнейших направлений развития. Вот вам яркий пример современных тенденций - консультация с широким активом в значительной степени обусловливает важность соответствующих условий активизации. В целом, конечно, новая модель организационной деятельности предопределяет высокую востребованность своевременного выполнения сверхзадачи.</p>

       <p>Кстати, ключевые особенности структуры проекта неоднозначны и будут ограничены исключительно образом мышления. В частности, существующая теория влечет за собой процесс внедрения и модернизации инновационных методов управления процессами! Идейные соображения высшего порядка, а также постоянное информационно-пропагандистское обеспечение нашей деятельности требует от нас анализа укрепления моральных ценностей. Современные технологии достигли такого уровня, что глубокий уровень погружения играет важную роль в формировании приоритизации разума над эмоциями. Предварительные выводы неутешительны: семантический разбор внешних противодействий позволяет выполнить важные задания по разработке экономической целесообразности принимаемых решений! С другой стороны, базовый вектор развития требует определения и уточнения распределения внутренних резервов и ресурсов.</p>

       <p>Приятно, граждане, наблюдать, как интерактивные прототипы могут быть подвергнуты целой серии независимых исследований. В своём стремлении повысить качество жизни, они забывают, что новая модель организационной деятельности, а также свежий взгляд на привычные вещи - безусловно открывает новые горизонты для распределения внутренних резервов и ресурсов.</p>
    </section>
    <section id="examples" class="cards">
      <div class="card">
        <h3>гордое название</h3>
      <p>Лишь акционеры крупнейших компаний, вне зависимости от их уровня, должны быть преданы социально-демократической анафеме. Интерактивные прототипы, инициированные исключительно синтетически, описаны максимально подробно. Принимая во внимание показатели успешности, реализация намеченных плановых заданий играет определяющее значение для новых принципов формирования материально-технической и кадровой базы. Как принято считать, ключевые особенности структуры проекта объективно рассмотрены соответствующими инстанциями.</p>
      <q-btn color="black" label="в личку напишу" />
      </div>
      <div class="card">
        <h3>гордое название</h3>
      <p>Лишь акционеры крупнейших компаний, вне зависимости от их уровня, должны быть преданы социально-демократической анафеме. Интерактивные прототипы, инициированные исключительно синтетически, описаны максимально подробно. Принимая во внимание показатели успешности, реализация намеченных плановых заданий играет определяющее значение для новых принципов формирования материально-технической и кадровой базы. Как принято считать, ключевые особенности структуры проекта объективно рассмотрены соответствующими инстанциями.</p>
      <q-btn color="black" label="в личку напишу" />
      </div>
      <div class="card">
        <h3>гордое название</h3>
      <p>Лишь акционеры крупнейших компаний, вне зависимости от их уровня, должны быть преданы социально-демократической анафеме. Интерактивные прототипы, инициированные исключительно синтетически, описаны максимально подробно. Принимая во внимание показатели успешности, реализация намеченных плановых заданий играет определяющее значение для новых принципов формирования материально-технической и кадровой базы. Как принято считать, ключевые особенности структуры проекта объективно рассмотрены соответствующими инстанциями.</p>
      <q-btn color="black" label="в личку напишу" />
      </div>
      <div class="card">
        <h3>гордое название</h3>
      <p>Лишь акционеры крупнейших компаний, вне зависимости от их уровня, должны быть преданы социально-демократической анафеме. Интерактивные прототипы, инициированные исключительно синтетически, описаны максимально подробно. Принимая во внимание показатели успешности, реализация намеченных плановых заданий играет определяющее значение для новых принципов формирования материально-технической и кадровой базы. Как принято считать, ключевые особенности структуры проекта объективно рассмотрены соответствующими инстанциями.</p>
      <q-btn color="black" label="в личку напишу" />
      </div>
    </section>
    <section id="contacts" class="contacts">
      <div class="q-pa-md" style="max-width: 400px">

          <q-form
            @submit="onSubmit"
            @reset="onReset"
            class="q-gutter-md"
          >
            <q-input
              rounded
              v-model="name"
              label="Your name *"
              hint="Name and surname"
              lazy-rules
              :rules="[ val => val && val.length > 0 || 'Please type something']"
            />

            <q-input
             v-model="email"
             rounded
             type="email"
             label="E-mail ** - прям вообще обязательно"
             hint="Email" />

            <q-toggle v-model="accept" label="не робот я вообще" />

            <div>
              <q-btn label="хочу текст" type="submit" color="primary"/>
              <q-btn label="передумал, я спать" type="reset" color="primary" flat class="q-ml-sm" />
            </div>
          </q-form>

        </div>
    </section>
  </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex'
}
</script>

<style lang="scss">
body{
  margin: 0 auto;
  width: 80%;
}
.main {
  height: 600px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: relative;
}
.main:after {
    content : "";
    display: block;
    position: absolute;
    top: 0;
    left: 0;
    background-image: url(../assets/main-background_pisanina.jpg);
    background-position: center;
    background-size: 100% 100%;
    width: 100%;
    height: 100%;
    opacity : 0.85;
    z-index: -1;
}
.avatar{
  border-radius: 50%;
  width: 300px;
  top: 15px;
  left: 15px;
}
.cards{
  display: flex;
  flex-direction: row;

  p {
    padding: 15px;
  }
}
.contacts{
  height: 600px;
  background-image: url(../assets/contact-background.jpg);
  background-position: center;
  background-size: 100% 100%;
}
</style>
