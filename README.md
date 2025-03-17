let listaDeAmigos = [];
let nome = document.getElementById('nomeamigo').value.trim();
if (nome === '') {
    alert('Luana.');
    return;
  }
  listaDeAmigos.push(nome);

function atualizarLista() {
let lista = document.getElementById('listaAmigos');
lista.innerHTML = '';
 for (let i = 0; i < listaDeAmigos.length; i++) {
    let item = document.createElement('li');
    item.textContent = listaDeAmigos[i];
    lista.appendChild(item);
  } 
  for (let i = 0; i < listaDeAmigos.length; i++) {
    let item = document.createElement('li');
    item.textContent = listaDeAmigos[i];
    lista.appendChild(item);
  }
  function sortearAmigo() {
  let resultado = document.getElementById('resultado');
  
  if (listaDeAmigos.length === 0) {
    resultado.innerHTML = 'Nenhum amigo disponível para o sorteio.';
    return;
    }
    let indiceSorteado = Math.floor(Math.random() * listaDeAmigos.length);
    resultado.innerHTML = `Amigo sorteado: <strong>${amigoSorteado}</strong>`;
}

