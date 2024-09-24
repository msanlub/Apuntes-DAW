# Autenticación SSH

Para saber si tenemos alguna ssh ya configurada, desde terminal `ls -al ~/.ssh`

### Crear desde 0

1. Me coloco en directorio .ssh -> `cd ~/,ssh`
2. Creo un mail -> `ssh -Heygen -+ ed25519 -C "email"
	- id_rsa (id clave pública)
	- passphrase (vacío)
	- se genera una clave ssh.pub (público)
3. Consigo el ide del ssh -> ` eval "$(ssh-agent -s)"`
4. Abrir el fichero de configuración -> ` touch ~/.ssh/config'
	-> copio y pego el host que viene en los pasos con mi id (id_rsa)
5. Añadir -> ` ssh -add --aple -use -Keychain ~/.ssh/id_rsa`
6. Vamos a GitHub, a nuestro usuario -> setting -> SSH -> New key -> cogemos la clave pública de la carpeta ssh (id_rsa.pub) -> lo añado.
7. Probar -> `ssh -T git@github.com`/Yes / comprobar de nuevo.