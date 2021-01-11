<template>
  <div>
    <!-- As a heading -->
    <b-navbar class="nabvar-bbva" variant="faded">
      <img src="../assets/img/logo.png" />
    </b-navbar>
    <div class="container content-controllers">
      <div class="row">
        <div class="col-sm-3">
          <select class="select-bbva">
            <option>Productos</option>
          </select>
          <div class="content-text-info-select">
            <img src="../assets/img/info.png" />
            <label>Seleciona una producto</label>
          </div>
        </div>
        <div class="col-sm-3">
          <select class="select-bbva">
            <option>Divisiones</option>
          </select>
          <div class="content-text-info-select">
            <img src="../assets/img/info.png" />
            <label>Seleciona una división</label>
          </div>
        </div>
        <div class="col-sm-3">
          <select class="select-bbva">
            <option>Zonas</option>
          </select>
          <div class="content-text-info-select">
            <img src="../assets/img/info.png" />
            <label>Seleciona una zona</label>
          </div>
        </div>
        <div class="col-sm-3">
          <select class="select-bbva">
            <option>Sucursales</option>
          </select>
          <div class="content-text-info-select">
            <img src="../assets/img/info.png" />
            <label>Seleciona una sucursal</label>
          </div>
        </div>
      </div>
      <hr />
    </div>
    <div class="container">
      <md-table class="md-elevation-1">
        <md-table-row>
          <md-table-head>CR División</md-table-head>
          <md-table-head>Nombre de la División</md-table-head>
          <md-table-head>Día T-2</md-table-head>
          <md-table-head>Día T-1</md-table-head>
          <md-table-head>Día actual</md-table-head>
          <md-table-head>Saldo Real</md-table-head>
          <md-table-head>Presupuesto</md-table-head>
          <md-table-head>Logro Equivalente (%)</md-table-head>
        </md-table-row>

        <md-table-row>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
        </md-table-row>

        <md-table-row>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
        </md-table-row>
      </md-table>

      <md-table class="md-elevation-1">
        <md-table-row>
          <md-table-head>Faltante fin de mes 90%</md-table-head>
          <md-table-head>Faltante fin de mes 100%</md-table-head>
          <md-table-head>Meta hoy 90%</md-table-head>
          <md-table-head>Meta hoy 100%</md-table-head>
          <md-table-head>Ritmo diario 90%</md-table-head>
          <md-table-head>Ritmo diario 100%</md-table-head>
          <md-table-head>Promedio Per Capita</md-table-head>
          <md-table-head>Eje en 0's</md-table-head>
        </md-table-row>

        <md-table-row>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
        </md-table-row>

        <md-table-row>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
          <md-table-cell>0000</md-table-cell>
        </md-table-row>
      </md-table>
    </div>
  </div>
</template>

<script>
import Vue from 'vue'
import VueMaterial from 'vue-material'
// Vue material
import 'vue-material/dist/vue-material.min.css'
import 'vue-material/dist/theme/default.css'

Vue.use(VueMaterial)
export default {
  props: {
    msg: String
  }
}
</script>

<style>
@import '../assets/css/fonts.css';

hr {
  background: #D3D3D3;
  margin-top: 32px !important;
  margin-bottom: 32px !important;
}

.nabvar-bbva {
  background: #072146;
  padding-top: 16px !important;
  padding-bottom: 16px !important;
}

.nabvar-bbva img {
  width: 10%;
}

.content-controllers {
  margin-top: 32px;
}

.select-bbva {
  width: 100%;
  border: none;
  border-bottom: 1px solid #666;
  font-size: 15px;
  padding-left: 8px;
  padding-top: 16px;
  padding-bottom: 16px;
  color: #666666;
  background: #ffffff;
  letter-spacing: 0;
  font-family: 'BentonSansBBVA-Book';
}

.select-bbva:focus {
  border: none !important;
}

.content-text-info-select {
  padding-left: 8px;
}

.content-text-info-select label {
  font-size: 13px;
  color: #121212;
  margin: 0px;
  letter-spacing: 0;
  font-family: 'BentonSansBBVA-Book';
}

.content-text-info-select img {
  width: 6%;
  margin-right: 4px;
}

.md-table {
  margin-bottom: 32px;
}

.md-table-head-label {
  color: #121212;
  font-size: 12px;
  font-family: 'BentonSansBBVA-Medium';
  letter-spacing: 0;
}

.md-table-cell-container {
  color: #666666;
  font-size: 13px;
  font-family: 'BentonSansBBVA-Book';
}

@media (min-width: 1200px) {
  .container {
    max-width: 1340px !important;
  }
}
</style>