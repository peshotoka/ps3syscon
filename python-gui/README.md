# Python-gui
Python GUI version of the cli 'ps3_syscon_uart_script.py'

## Build a compiled EXE for Linux and Windows using Pyinstaller

NOTE: Make sure to have the 'pyserial and pycryptodomex' python modules installed!
Also for linux users - package tkinter needs to be installed!

`pip install pyinstaller`

From the cmd line:

### Linux

`pyinstaller --noconfirm --onefile --console --clean --add-data "gui_diag_serial.py:." --hidden-import "Cryptodome.Cipher.AES"  "gui_ps3_syscon_uart_script.py"`

### Windows

`pyinstaller --noconfirm --onefile --console --clean --add-data "gui_diag_serial.py;." --hidden-import "Cryptodome.Cipher.AES"  "gui_ps3_syscon_uart_script.py"`