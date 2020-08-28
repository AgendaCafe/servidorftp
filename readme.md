# Servidor FTP

Criar senha no terminal:
/bin/echo "{md5}"`/bin/echo -n "senha" | openssl dgst -binary -md5 | openssl enc -base64`

Criar senha em PHP:
$password = "{md5}".base64_encode(pack("H*", md5("senha")));