const input = document.getElementById('pin');

const pw = 123;
let saldo = 10000000; //10jt

const cash = {
  seratus: '100000',
  duaratus: '200000',
  tigaratus: '300000',
  limaratus: '500000',
  satujuta: '1000000',
  satusetengah: '1500000',
  duajuta: '2000000',
};

function masuk() {
  if (input.value == pw) {
    window.location.href = '../pages/jumlah.html';
  } else {
    alert('pin salah');
  }
}

function tunai(value) {
  if (saldo >= value && confirm('anda ingin narik saldo') == true) {
   alert(`kamu menarik saldo ${value} sisa saldo kamu ${saldo = saldo-value}`)
  } else {
    alert('gagal');
  }
}
