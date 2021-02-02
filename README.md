# banrep_col_Uipath


Url: https://totoro.banrep.gov.co/analytics/saw.dll?Go


Requirements:

-Use ReFramework

-No queues


-Use Assets to configure: url, exit and entry roots (ruras de salida y entrada), email credentials from which the report will be sent


1-directory structure on path: "C:\users\...\Documents\robot" structured as follows:


Archivos_Recibidos:

Base:

Logs:

Trazabilidad:

from the Banco de la republica page  must be downloaded in csv format the followinf data:

a- informe de la tasa representativa de cambio cop-usd  1-1-2020 31-12-2020

b-... cop-euros 1-1-2020 31-12-2020

con cada archivo debe calcularse promedio anual c/year, valor maximo y val minimo c/year, promedio general de la TRM y que mes presento el valor maximo y minimo.

Realizar xlm con 3 hojas con los informes, el xml debe ser enviado por correo




-The TransactionItem variable in the Main file should be of the System.Data.DataRow type, as we are extracting the entire table to process it one row at a time. You should also change the argument type in the GetTransactionData, Process and SetTransactionStatus workflows to match the TransactionItem type.

-Remove the three SetTransactionStatus activities from the SetTransactionStatus workflow as we are not using the transaction functionality provided by Orchestrator.



-Change log location:
It is possible to change the default location of UiPath Studio log files. To do this, open the file UiPath.Studio.exe.config. This file is located inside the installation folder of UiPath.

For example, C:\Users\<username>\AppData\Local\UiPath\app-19.2.0\UiPath.Studio.exe.config

Open this config file using any text editor such as a Notepad.

Simply change the value of the logDirectory parameter. This can be found under the nlog tag. The value of the logDirectory parameter is set to %LocalApplicationData%\UiPath\Logs. Update this location to reflect the desired location to save the logs.
