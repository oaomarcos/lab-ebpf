
📘 Índice

1. Configuração inicial
   
- Subir a topologia com os dois nós (node-a e node-b).

- Verificar endereços IP configurados com ip addr show.

- Testar conectividade básica com ping.

2. Captura de pacotes

- Executar tcpdump -i eth1 em node-a para observar tráfego.

- Gerar tráfego com ping e verificar pacotes ICMP capturados.

- Salvar captura em arquivo (tcpdump -i eth1 -w ping.pcap) e analisar depois com Wireshark.

3. Análise de tráfego

- Comparar pacotes ICMP de requisição e resposta.

- Identificar cabeçalhos IP e campos relevantes (TTL, checksum).

- Discutir como o tráfego é roteado dentro da sub-rede.

4. Testes com ferramentas adicionais

- Usar iperf3 para medir largura de banda entre os nós.

- Usar netcat para simular conexões TCP e UDP.

- Explorar dig ou nslookup para consultas DNS (mesmo em rede simples).

5. Simulação de falhas

- Derrubar a interface (ip link set eth1 down) e observar impacto.

- Alterar máscara de rede para valores incorretos e analisar perda de conectividade.

- Usar tcpdump para verificar ausência de tráfego.

6. Documentação e relatório

- Cada grupo deve registrar comandos utilizados, capturas e conclusões.

- Comparar resultados entre grupos e discutir boas práticas de análise.
