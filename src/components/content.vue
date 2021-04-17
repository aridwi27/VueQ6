<template>
  <div class="col-9">
    <h1 class="my-5 font-weight-bold">Task For Today</h1>
    <div class="row">
      <b-button v-b-modal.modal-lg class="btncreate ml-3 mr-5 col-2"
        ><b-icon
          icon="plus"
          font-scale="1.5"
          aria-hidden="true"
          class="mr-1"
        ></b-icon
        >Create New</b-button
      >
      <input
        type="email"
        class="form-control d-inline col-9 formsearch text-center"
        placeholder="Cari"
      />
    </div>
    <div class="card w-100 my-5">
      <div class="card-body">
        <h5 class="card-title font-weight-bold">Daily Stand Up</h5>
        <p class="card-text d-inline">
          1. Dont forget prepare your report and any blocker in Front end.<br />
          2. Telling Project Manager for new assignment.
        </p>
        <b-icon
          icon="trash-fill"
          font-scale="1"
          aria-hidden="true"
          class="d-inline float-right mx-3"
        ></b-icon>
        <b-icon
          icon="pen-fill"
          font-scale="1"
          aria-hidden="true"
          class="d-inline float-right"
        ></b-icon>
      </div>
    </div>
    <div class="card w-100 my-5">
      <div class="card-body">
        <h5 class="card-title font-weight-bold">Meeting With Client A</h5>
        <p class="card-text d-inline">
          1. Loream Ipsum Dolor Amet <br />
          2. Loream Ipsum Dolor Amet
        </p>
        <b-icon
          icon="trash-fill"
          font-scale="1"
          aria-hidden="true"
          class="d-inline float-right mx-3"
        ></b-icon>
        <b-icon
          icon="pen-fill"
          font-scale="1"
          aria-hidden="true"
          class="d-inline float-right"
        ></b-icon>
      </div>
    </div>
    <div class="card w-100 my-5">
      <div class="card-body">
        <h5 class="card-title font-weight-bold">Meeting With Client B</h5>
        <p class="card-text d-inline">
          1. Loream Ipsum Dolor Amet <br />
          2. Loream Ipsum Dolor Amet
        </p>
        <b-icon
          icon="trash-fill"
          font-scale="1"
          aria-hidden="true"
          class="d-inline float-right mx-3"
        ></b-icon>
        <b-icon
          icon="pen-fill"
          font-scale="1"
          aria-hidden="true"
          class="d-inline float-right"
        ></b-icon>
      </div>
    </div>

    <!-- modal -->
    <b-modal
      hide-header
      hide-footer
      id="modal-lg"
      size="lg"
      title="Large Modal"
    >
      <div class="px-5">
        <h4 class="font-weight-bold">New Task</h4>
        <form>
          <div class="form-group my-5">
            <label for="tittle"><h4 class="font-weight-bold">Tittle</h4></label>
            <input
              type="text"
              class="form-control"
              id="tittle"
              placeholder="Fill Tittle"
            />
          </div>
          <div class="form-group">
            <label for="description"
              ><h4 class="font-weight-bold">Description</h4></label
            >
            <textarea
              type="text"
              class="form-control"
              id="description"
              rows="4"
              placeholder="Fill Description"
            />
          </div>
          <div class="form-group my-5">
            <h4 class="font-weight-bold">Choose Date</h4>
            <b-calendar
              v-model="value"
              @context="onContext"
              class="ml-4"
            ></b-calendar>
          </div>
          <div class="text-center">
            <button type="button" class="btn btn-outline-light colorbtn btn-lg">
              Cancel
            </button>
            <button
              type="button"
              class="btn btn-secondary btn-lg btnmodalcreate mx-3"
            >
              Create Task
            </button>
          </div>
        </form>
      </div>
    </b-modal>
  </div>
</template>

<style scoped>
.btncreate {
  background: #0442d0;
  border-radius: 15px;
}
.formsearch {
  border: 1px solid #0442d0;
  box-sizing: border-box;
  border-radius: 15px;
}
.btnmodalcreate {
  background: #0442d0;
  border-radius: 10px;
}
.colorbtn {
  color: #0442d0;
}
</style>
