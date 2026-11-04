# Instalacija Pythona i prvi program

Najkraći put do pokretanja Pythona na vašem računalu.

## Usporedba po sustavima

| Operacijski sustav | Instalacija | Naredba za provjeru |
| :--- | :--- | :--- |
| **Windows** | Preuzmite installer s [python.org](https://www.python.org/). Obavezno označite opciju **"Add python.exe to PATH"**. | `python --version` |
| **macOS** | Preuzmite paket s [python.org](https://www.python.org/) ili instalirajte preko Homebrewa: `brew install python`. | `python3 --version` |

## Provjera instalacije

Otvorite terminal i pokrenite:

```bash
python --version
```
### Prvi program

```
touch program.py
echo "print('Hello World')">> program.py
```

Pokrenite ga sa:
```python program.py```
