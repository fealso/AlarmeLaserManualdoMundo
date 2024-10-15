# AlarmeLaserManualdoMundo
Sistema de Alarme a Laser com Arduino 🚨🔦

Este projeto é um sistema de alarme a laser desenvolvido com Arduino. Ele utiliza um módulo LDR (sensor de luz) para detectar quando o feixe de laser é interrompido. Quando a luz do laser é bloqueada, um relé ativa o alarme (que pode ser um buzzer ou outro dispositivo), e o sistema só será reiniciado quando um botão for pressionado, desativando o alarme.

Principais Funcionalidades:
Sensor de Luz (LDR): Detecta a interrupção do feixe de laser.
Relé para Controle do Alarme: Aciona o alarme (buzzer, lâmpada, etc.) quando o feixe de laser é interrompido.
Botão de Reinício: Permite desativar o alarme manualmente e reiniciar o sistema.
Monitoramento Serial: Exibe o valor da luz e o estado do sistema para depuração em tempo real (opcional).

Como Funciona:
O sistema monitora continuamente o valor do sensor LDR.
Quando o valor do LDR indica que a luz foi interrompida, o relé é ativado e o alarme dispara.
O alarme continua ativo mesmo que a luz seja restaurada até que o botão de desarme seja pressionado.
Pressionando o botão, o alarme é desativado e o sistema é reiniciado, aguardando uma nova interrupção do feixe de laser.

Componentes Utilizados:
Arduino Uno ou similar
Módulo LDR para detecção de luz (saída digital)
Módulo Relé para controle do alarme
Botão para desarmar o alarme
Laser para ser direcionado ao LDR
Buzzer ou outro dispositivo de alarme

Melhorias Futuras (que pensamos em fazer):
Adicionar temporizadores para tempo de disparo do alarme.
Integração com displays LCD ou LEDs para mostrar o estado do sistema.
Controle remoto via Bluetooth ou Wi-Fi para monitoramento e controle do alarme.
