## Opis / Description:

Ten projekt umożliwia automatyczne nawiązywanie połączeń z platformą Command & Control (C2) oraz hostowanie interfejsu API bez bezpośredniego dostępu do API. Skrypt wykorzystuje bibliotekę paramiko do bezpiecznych połączeń SSH oraz framework Flask do obsługi żądań API.

This project enables automatic connection establishment with a Command & Control (C2) platform and hosting an API interface without direct API access. The script uses the paramiko library for secure SSH connections and the Flask framework for handling API requests.

[![Kliknij tutaj](https://cdn.discordapp.com/attachments/1217082239494389871/1239333324040700025/standard.gif?ex=667fd85a&is=667e86da&hm=6575a51692da886a9e81aead1ccddb7cf88c2a8b02dcb2e99c8df8743bb309a1&)](https://discord.gg/j4485Q3R)

**CLICK ME**

[Discord](https://discord.gg/j4485Q3R) | [Telegram](https://t.me/heroinprojects)

---

### Instrukcje / Instructions:

1. Pobierz i zainstaluj niezbędne biblioteki, wykonując polecenie / Install the required libraries by executing the command:
pip install paramiko flask

2. Skonfiguruj plik `config.ini`, w którym należy określić / Configure the `config.ini` file, where you need to specify:
- `host` i `port` platformy C2, które będą używane domyślnie przez aplikację / `host` and `port` of the C2 platform that will be used by default by the application.

Przykładowa zawartość pliku `config.ini` / Example `config.ini` content:
[DEFAULT]
host = <adres_hosta_C2>
port = <port_C2>

3. Uruchom aplikację, uruchamiając plik `sshconnect.py`. Aplikacja będzie dostępna pod adresem / Run the application by executing the `sshconnect.py` file. The application will be accessible at:

Wzór api / Api template
localhost:5000/api/attack?username=<username>&key=<key-password>&host=<ip what you want to atack>&port=<attack port>&time=<attack time>&method=<attack method>
