<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <h2 class="text-center my-4">RIWAYAT KUNJUNGAN</h2>
        <div class="my-3">
          <input type="search" class="form-control form-control-lg rounded-5" placeholder="Filter...">  
        </div>
        <div class="my-3 text-muted">menampilkan 1 dari 1</div>
        <table class="table">
          <thead>
            <tr>
              <td>#</td>
              <td>NAMA</td>
              <td>KEANGGOTAAN</td>
              <td>KELAS</td>
              <td>WAKTU</td>
              <td>KEPERLUAN</td>
            </tr>   
          </thead>  
          <tbody>
            <tr>
              <td>1.</td>
              <td>Rm</td>
              <td>siswa</td>
              <td>11pplg2</td>
              <td>24 Febuari 2024, 23.31.00</td>  
              <td>Baca</td>
            </tr>
          </tbody>
          <tbody>
            <tr>
              <td>2.</td>
              <td>mo</td>
              <td>siswa</td>
              <td>10pplg1</td>
              <td>24 Febuari 2024, 23.31.00</td>  
              <td>pinjam buku</td>
            </tr>
          </tbody>
        </table>
      </div>  
    </div>
  </div> 
  <Nuxt-Link to="/"> 
               <button type="submit" class="btn btn-secondary btm-lg rounded-5" style="margin-left: 82%;" >BACK</button>
               </Nuxt-Link>
</template>

<script setup>
const supabase = useSupabaseClient()

const visitors = ref([])
const getPengunjung = async () => {
  const { data, error } = await supabase.from('pengunjung').select('*, keanggotaan(*), keperluan(*)')
  if(data) visitors.value =data
  }

  onMounted(() => {
    getPengunjung()
  })
</script>
