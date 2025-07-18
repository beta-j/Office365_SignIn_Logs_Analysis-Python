I created this Python script to analyse the Office365 sign-in log files which are generated in CSV format.

To use the script simply place the csv files in a sub-folder called `O365_temp` in the same folder as the .ipynb file.  Then run the ipynb using your preferred software - I normally use Visual Basic or Jupyter Notebook.

There are two variables in the **Initialise Environment** block that you may wish to populate: `sensitive_users` holds a list fo user names for security-sensitive employees (eg. sys admins, managers, CEO, etc..), while `safe_ips` is a comma-seperated list of known safe IP addresses - typically these would be your company's public facing IPs and those of trusted third parties.

**Note:** The script uses `pandas`, `matlplotlib` and `seaborn` which you need to install to your python environment in advance.
