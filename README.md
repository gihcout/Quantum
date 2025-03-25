Repositório criado para salvar os conteúdos de estudo sobre computação quântica.

&nbsp;

```python
from qiskit import QuantumCircuit
from qiskit_aer import AerSimulator

# Criando um circuito quântico com 1 qubit e 1 bit clássico
circuit = QuantumCircuit(1, 1)
circuit.h(0)
circuit.measure(0, 0)

simulator = AerSimulator()
result = simulator.run(circuit, shots=1000).result()
counts = result.get_counts(circuit)
print("Resultado da medição:", counts)
```
&nbsp;

## 

<p style="color:rgb(55, 101, 200); font-size: 18px; font-variant: small-caps">Conceitos de Computação Quântica</p>

**O que são os Qubits?**

Qubits são os bits quânticos, a unidade fundamental de informação na computação quântica. Diferente dos bits clássicos, que podem ter apenas os valores 0 ou 1, os qubits podem estar simultaneamente nos dois estados, ou em uma combinação desses estados. Isso ocorre devido à superposição, o que aumenta exponencialmente a capacidade de processamento de informações em sistemas quânticos.

**O que é a Superposição?**

Superposição é o fenômeno quântico que permite que um qubit esteja em múltiplos estados ao mesmo tempo, ao invés de estar em apenas um estado clássico. Quando realizado o processo de medição, o qubit "colapsa" para um dos dois estados possíveis, escolhidos com base em probabilidades. Esse fenômeno permite que um computador quântico execute cálculos em várias possibilidades simultaneamente, potencialmente resolvendo problemas muito mais rapidamente do que um computador clássico.

**O que é o Entrelaçamento?**

O entrelaçamento quântico é um fenômeno em que dois ou mais qubits se tornam interdependentes de tal maneira que o estado de um qubit não pode ser descrito independentemente do estado dos outros. Em outras palavras, a medida de um qubit afetará instantaneamente o estado de outros qubits entrelaçados, independentemente da distância que os separa. Uma vez entrelaçadas, se você medir uma das partículas, o estado da outra partícula será instantaneamente determinado, mesmo que estejam a grandes distâncias. Esse entrelaçamento cria uma ligação única e "instantânea" entre os qubits.

**Porque esses entrelaçamentos são sensíveis?**

O entrelaçamento quântico é extremamente sensível a interferências externas, como campos magnéticos, flutuações de temperatura, vibrações, entre outros fatores. Essas condições podem interromper a ligação quântica entre as partículas, o que faz com que o entrelaçamento seja perdido, um fenômeno chamado decoerência quântica. Isso é um grande desafio para a computação quântica, pois a transferência de estado quântico depende dessa ligação estável entre os qubits. E essa questão é um dos desafios dos sistemas quânticos.


[<img width="45" src="https://github.com/gihcout/arduino/assets/112673878/a25404ac-e2a0-4e53-9f31-3a55b0bdfebc" />](https://github.com/gihcout)