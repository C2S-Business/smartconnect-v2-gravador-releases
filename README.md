# Gravador SmartConnect V2

Este repositório público guarda somente os instaladores e as atualizações do
gravador. **O firmware e as credenciais MQTT não fazem parte das releases.**

## Instalar

Baixe a [última release](https://github.com/C2S-Business/smartconnect-v2-gravador-releases/releases/latest):

- **Windows:** `SmartConnect-V2-Gravador-Windows-Setup.exe`. Instala no perfil do usuário e cria um atalho no menu Iniciar.
- **macOS:** `SmartConnect-V2-Gravador-macOS.dmg`. Arraste o aplicativo para Applications. O app é assinado e notarizado pela C2S Business.

Ao abrir pela primeira vez, use **Importar firmware privado...** para escolher
o `.hex` oficial recebido da C2S. Conecte a placa via USB, selecione a porta,
clique em **Preparar**, pressione e solte **RESET** na placa e clique em
**Gravar** imediatamente. O aplicativo usa AVRDUDE e verifica a gravação.

O aplicativo consulta novas releases ao abrir. Quando houver uma versão nova,
ele oferece a atualização e verifica o SHA-256 do instalador baixado. O
firmware importado é preservado durante a atualização.

O gravador é destinado às placas SmartConnect V2 com bootloader serial
`arduino` a 115200 baud. Feche o Monitor Serial antes de gravar.
