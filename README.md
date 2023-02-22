# -Icarus1
Código que verifica se ocorre a necessidadede atualizações. Agora como efetuar se há atualizações disponíveis para o SO utilizando a API do Windows UpdadeAPI por um boot em pendrive ?


include iostream

include string

using namespace std;

// Função para checar se a máquina precisa de atualizações

bool precisaAtualizar(string maquina)

{

    // Aqui pode ser implementada a lógica para verificar se a máquina precisa de atualizações
    // De forma simples, nessa lógica, apenas retornamos true se o nome da máquina tiver o caracter '1'
return (maquina.find('1') != string::npos);
}
int main() {

    // Identificar a máquina
    
    string nomeMaquina = "Maquina2"; // Exemplo de nome de máquina
    

    // Verificar se a máquina precisa de atualizações
    bool precisaAtualizacao = precisaAtualizar(nomeMaquina);

    // Imprimir informações na tela
    cout << "Nome da maquina: " << nomeMaquina << endl;
    if (precisaAtualizacao) {
        cout << "A maquina precisa de atualizacoes." << endl;
    }
       }
    else {
        cout << "A maquina nao precisa de atualizacoes." << endl;
    }

    return 0;
}
