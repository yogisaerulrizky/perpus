<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <h2 class="text-center my-4">ISI BUKU KUNJUNGAN</h2>
        <from>
          <div class="mb-3">
            <input type="text" class="form-control from-control-lg rounded-5" placeholder="NAMA...">
          </div>
          <div class="mb-3">
            <select class="from-control from control-lg from-select rounded">
              <option value="">KEANGGOTAAN</option>
              <option value="Siswa">Siswa</option>
              <option value="Guru">Guru</option>
              <option value="Staf">Staf</option>
              <option value="Umum">Umum</option>
            </select>
          </div>
          <div class="mb-3">
            <div class="row">
              <div class="col-md-4">
                <select class="form-control from-control-lg from-select rounded-5 mb-2">
                  <option value="">TINGKAT</option>
                  <option value="X">X</option>
                  <option value="XI">XI</option>
                  <option value="XII">XII</option>
                </select>
              </div>
              <div class="col-md-4">
                <select class="from-control from-control-lg from-select rounded-5 mb-2">
                  <option value="">JURUSAN</option>
                  <option value="PPLG">PPLG</option>
                  <option value="TJKT">TJKT</option>
                  <option value="TSM">TSM</option>
                  <option value="DKV">DKV</option>
                  <option value="TOI">TOI</option>
                </select>
              </div>
              <div class="col-md-4">
                <select class="form-control form-control-lg form-select rounded-5" mb-2>
                  <option value="">KELAS</option>
                  <option value="1">1</option>
                  <option value="2">2</option>
                  <option value="3">3</option>
                  <option value="4">4</option>            
                </select>
              </div>
             value=</div>
          </div>
          <div class="mb-3">
            <select class="form-control form-control-lg form-select rounded-5">
              <option value="">KEPERLUAN</option>
              <option value="baca">Baca Buku</option>
              <option value="Pinjam">Pinjam Buku</option>
              option >Kembalikan Buku  /option>
            </select>
          </div>
          <button type="submit" class="btn btn-dark btn-lg rounded-5 px-5">KIRIM</button>
        </from>
      </div>
    </div>
  </div>
</template>