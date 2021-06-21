# ansible_iosXR_devnetBOX
## Devnet Lab
O laboratorio devnet utilizado foi: https://devnetsandbox.cisco.com/RM/Diagram/Index/883f8ea6-54a1-453e-98f5-fc175a2a90de?diagramType=Topology
É neccessario reserva-la, você pode reserva-la por até uma semana, geralmente se leva 10 minutos para a configuração da mesma terminar, você receberá um email com o endereço do servidor vpn da box(você precisa se conectar a vpn provida para poder acessar o laboratorio), login e senha.
## Execução do script
A unica dependencia desse script realmente é o ansible, que pode ser facilmente instalado com um
```sudo package-manager install ansible -y```
Para executar o script o comando é
```ansible-playbook ./main.yml --tags=basic_port_config --extra-vars "interface=nome da interface alvo ip=ip a ser configurado mask=mascara a ser configurada"```
