<template>
  <div class="col-3 mt-5">
    <div class="card cardsidebar mb-5" style="width: 20rem">
      <div class="card-body cardsidebar">
        <div class="row">
          <div class="col-4">
            <img src="../assets/images/todo.png" alt="" />
          </div>
          <div class="col-8">
            <h4 class="colorfont">Hallo, Sam!</h4>
            <p class="text-white">
              You have 2 tasks left for today, Already completed Task today?
            </p>
          </div>
        </div>
      </div>
    </div>
    <b-calendar v-model="value" @context="onContext" class="ml-4"></b-calendar>
  </div>
</template>

<style scoped>
.cardsidebar {
  background: #0442d0;
  border-radius: 20px;
}
.colorfont {
  color: #fabe2c;
}
.b-calender {
  width: 500px;
}
</style>
