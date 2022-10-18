```python
from sqlpd import DataBase
import pandas as pd
df = pd.read_excel('/mnt/Work/haoborn/tmp/anag_real_pdvs.xlsx', index_col=0)
```


```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>pdv_unique_id</th>
      <th>pdv_name</th>
      <th>pdv_stage</th>
      <th>pdv_nation</th>
      <th>pdv_CAP</th>
      <th>pdv_contact_1</th>
      <th>pdv_contact_2</th>
      <th>pdv_contact_3</th>
      <th>pdv_contact_4</th>
      <th>pdv_legacy_type</th>
      <th>...</th>
      <th>first_valid_progw</th>
      <th>last_progw</th>
      <th>progw_new_data_flow</th>
      <th>last_load_date</th>
      <th>progw_last_train_ml</th>
      <th>progw_last_model_selection</th>
      <th>last_sale_date</th>
      <th>last_order_date</th>
      <th>last_inventory_date</th>
      <th>pdv_corefa_id</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>pdv00001</td>
      <td>former_pdv11</td>
      <td>RapidTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>A</td>
      <td>...</td>
      <td>165.0</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-18 11:18:28</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17</td>
      <td>2022-07-17</td>
      <td>2022-07-03</td>
      <td>RyzenC</td>
    </tr>
    <tr>
      <th>1</th>
      <td>pdv00002</td>
      <td>former_pdv12</td>
      <td>RapidTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>A</td>
      <td>...</td>
      <td>210.0</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17 01:35:31</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17</td>
      <td>2022-07-17</td>
      <td>2022-07-03</td>
      <td>RyzenC</td>
    </tr>
    <tr>
      <th>2</th>
      <td>pdv00003</td>
      <td>former_pdv21</td>
      <td>AlphaTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>A</td>
      <td>...</td>
      <td>165.0</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-18 11:18:28</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17</td>
      <td>2022-07-17</td>
      <td>2022-07-03</td>
      <td>RyzenD</td>
    </tr>
    <tr>
      <th>3</th>
      <td>pdv00004</td>
      <td>former_pdv22</td>
      <td>AlphaTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>A</td>
      <td>...</td>
      <td>210.0</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17 01:35:31</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17</td>
      <td>2022-07-17</td>
      <td>2022-07-03</td>
      <td>RyzenD</td>
    </tr>
    <tr>
      <th>4</th>
      <td>pdv00005</td>
      <td>former_pdv31</td>
      <td>PreBetaTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>A</td>
      <td>...</td>
      <td>165.0</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-18 11:18:28</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17</td>
      <td>2022-07-17</td>
      <td>2022-07-03</td>
      <td>RyzenA</td>
    </tr>
    <tr>
      <th>5</th>
      <td>pdv00006</td>
      <td>former_pdv32</td>
      <td>PreBetaTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>A</td>
      <td>...</td>
      <td>210.0</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17 01:35:31</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17</td>
      <td>2022-07-17</td>
      <td>2022-07-03</td>
      <td>RyzenA</td>
    </tr>
    <tr>
      <th>6</th>
      <td>pdv00007</td>
      <td>former_pdv4</td>
      <td>PreBetaTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>B</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>7</th>
      <td>pdv00008</td>
      <td>first_LegD_pdv</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>8</th>
      <td>pdv00009</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>9</th>
      <td>pdv00010</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>10</th>
      <td>pdv00011</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>11</th>
      <td>pdv00012</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>12</th>
      <td>pdv00013</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>13</th>
      <td>pdv00014</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>14</th>
      <td>pdv00015</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>15</th>
      <td>pdv00016</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>16</th>
      <td>pdv00017</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>17</th>
      <td>pdv00018</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>18</th>
      <td>pdv00019</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>19</th>
      <td>pdv00020</td>
      <td>void</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>20</th>
      <td>pdv00021</td>
      <td>former_pdv01</td>
      <td>PreBetaTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>A</td>
      <td>...</td>
      <td>165.0</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-18 11:18:28</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17</td>
      <td>2022-07-17</td>
      <td>2022-07-03</td>
      <td>RyzenE</td>
    </tr>
    <tr>
      <th>21</th>
      <td>pdv00022</td>
      <td>former_pdv02</td>
      <td>PreBetaTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>A</td>
      <td>...</td>
      <td>210.0</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17 01:35:31</td>
      <td>498.0</td>
      <td>494.0</td>
      <td>2022-07-17</td>
      <td>2022-07-17</td>
      <td>2022-07-03</td>
      <td>RyzenE</td>
    </tr>
    <tr>
      <th>21</th>
      <td>pdv00023</td>
      <td>pdv_July2022</td>
      <td>PreBetaTest</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>A</td>
      <td>...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>NaT</td>
      <td>RyzenE</td>
    </tr>
  </tbody>
</table>
<p>23 rows × 36 columns</p>
</div>




```python
with DataBase.CreateConnection(db_user='mosesd',
                               db_pass='Moses1749',
                               db_host='127.0.0.1',
                               db_name='DPQ',
                               ssh_user='mdastmard',
                               ssh_pass='Moses1749',
                               ssh_host='80.211.60.172') as db:
    db.create_table("anag_real_pdvs", df)
```

    sshtunnel trying to connect to port 52491
    connection created.
    sshtunnel trying to connect to port 51359
    connection closed



    ---------------------------------------------------------------------------

    ModuleNotFoundError                       Traceback (most recent call last)

    /mnt/Work/github/sqlpd-package/Untitled.ipynb Cell 3 in <cell line: 1>()
          <a href='vscode-notebook-cell:/mnt/Work/github/sqlpd-package/Untitled.ipynb#ch0000001?line=0'>1</a> with DataBase.CreateConnection(db_user='mosesd',
          <a href='vscode-notebook-cell:/mnt/Work/github/sqlpd-package/Untitled.ipynb#ch0000001?line=1'>2</a>                                db_pass='Moses1749',
          <a href='vscode-notebook-cell:/mnt/Work/github/sqlpd-package/Untitled.ipynb#ch0000001?line=2'>3</a>                                db_host='127.0.0.1',
       (...)
          <a href='vscode-notebook-cell:/mnt/Work/github/sqlpd-package/Untitled.ipynb#ch0000001?line=5'>6</a>                                ssh_pass='Moses1749',
          <a href='vscode-notebook-cell:/mnt/Work/github/sqlpd-package/Untitled.ipynb#ch0000001?line=6'>7</a>                                ssh_host='80.211.60.172') as db:
    ----> <a href='vscode-notebook-cell:/mnt/Work/github/sqlpd-package/Untitled.ipynb#ch0000001?line=7'>8</a>     db.create_table("anag_real_pdvs", df)


    File /mnt/Work/github/sqlpd-package/sqlpd/src/database.py:182, in DataBase.Functions.create_table(self, table_name, df, *args, **kwargs)
        179 def create_table(self, table_name, df, *args, **kwargs):
        180     """ create a table in database specified in db_util
        181         by using the input dataframe """
    --> 182     engine = self.connection.get_engine()
        183     df = df.copy()
        184     df['chunk_id'] = range(len(df))


    File /mnt/Work/github/sqlpd-package/sqlpd/src/database.py:125, in DataBase.Connection.get_engine(self)
        124 def get_engine(self):
    --> 125     engine = create_engine(self.get_url())
        126     return engine


    File <string>:2, in create_engine(url, **kwargs)


    File ~/miniconda3/lib/python3.9/site-packages/sqlalchemy/util/deprecations.py:309, in deprecated_params.<locals>.decorate.<locals>.warned(fn, *args, **kwargs)
        302     if m in kwargs:
        303         _warn_with_version(
        304             messages[m],
        305             versions[m],
        306             version_warnings[m],
        307             stacklevel=3,
        308         )
    --> 309 return fn(*args, **kwargs)


    File ~/miniconda3/lib/python3.9/site-packages/sqlalchemy/engine/create.py:560, in create_engine(url, **kwargs)
        558         if k in kwargs:
        559             dbapi_args[k] = pop_kwarg(k)
    --> 560     dbapi = dialect_cls.dbapi(**dbapi_args)
        562 dialect_args["dbapi"] = dbapi
        564 dialect_args.setdefault("compiler_linting", compiler.NO_LINTING)


    File ~/miniconda3/lib/python3.9/site-packages/sqlalchemy/dialects/mysql/mysqldb.py:163, in MySQLDialect_mysqldb.dbapi(cls)
        161 @classmethod
        162 def dbapi(cls):
    --> 163     return __import__("MySQLdb")


    ModuleNotFoundError: No module named 'MySQLdb'



```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>server_class</th>
      <th>server_id</th>
      <th>server_ip_address</th>
      <th>server_SFTP_port</th>
      <th>server_FTP_port</th>
      <th>server_username</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>SYNCFA</td>
      <td>Aru1</td>
      <td>80.211.60.172</td>
      <td>21</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>1</th>
      <td>FRONTEFA</td>
      <td>Infinitech1</td>
      <td></td>
      <td>22</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>2</th>
      <td>INPUFA</td>
      <td>Ovh1</td>
      <td>149.202.46.231</td>
      <td>22</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>3</th>
      <td>INPUFA</td>
      <td>Ovh2</td>
      <td>149.202.46.231</td>
      <td>22</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>4</th>
      <td>COREFA</td>
      <td>Ovh3</td>
      <td></td>
      <td>22</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>5</th>
      <td>FRONTEFA</td>
      <td>Ovh4</td>
      <td></td>
      <td>22</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>6</th>
      <td>COREFA</td>
      <td>RyzenA</td>
      <td>95.229.102.51</td>
      <td>4040</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>7</th>
      <td>COREFA</td>
      <td>RyzenB</td>
      <td>95.229.102.51</td>
      <td>4050</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>8</th>
      <td>COREFA</td>
      <td>RyzenC</td>
      <td>95.229.102.51</td>
      <td>4060</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>9</th>
      <td>COREFA</td>
      <td>RyzenD</td>
      <td>95.229.102.51</td>
      <td>4070</td>
      <td>21</td>
      <td></td>
    </tr>
    <tr>
      <th>10</th>
      <td>COREFA</td>
      <td>RyzenE</td>
      <td>95.229.102.51</td>
      <td>4080</td>
      <td>21</td>
      <td></td>
    </tr>
  </tbody>
</table>
</div>




```python
# !pip install mysqlclient
```

    Collecting mysqlclient
      Downloading mysqlclient-2.1.1.tar.gz (88 kB)
    [K     |████████████████████████████████| 88 kB 524 kB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_bd4cb6dc834841b6b3828d4895cc9f93/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_bd4cb6dc834841b6b3828d4895cc9f93/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-xl69_jm6
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_bd4cb6dc834841b6b3828d4895cc9f93/
        Complete output (15 lines):
        mysql_config --version
        /bin/sh: 1: mysql_config: not found
        mariadb_config --version
        /bin/sh: 1: mariadb_config: not found
        mysql_config --libs
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_bd4cb6dc834841b6b3828d4895cc9f93/setup.py", line 15, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_bd4cb6dc834841b6b3828d4895cc9f93/setup_posix.py", line 70, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_bd4cb6dc834841b6b3828d4895cc9f93/setup_posix.py", line 31, in mysql_config
            raise OSError("{} not found".format(_mysql_config_path))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/50/5f/eac919b88b9df39bbe4a855f136d58f80d191cfea34a3dcf96bf5d8ace0a/mysqlclient-2.1.1.tar.gz#sha256=828757e419fb11dd6c5ed2576ec92c3efaa93a0f7c39e263586d1ee779c3d782 (from https://pypi.org/simple/mysqlclient/) (requires-python:>=3.5). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-2.1.0.tar.gz (87 kB)
    [K     |████████████████████████████████| 87 kB 1.9 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_d6fcfd51e48244b684a1f9a254001e48/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_d6fcfd51e48244b684a1f9a254001e48/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-zr5dlfkr
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_d6fcfd51e48244b684a1f9a254001e48/
        Complete output (15 lines):
        mysql_config --version
        /bin/sh: 1: mysql_config: not found
        mariadb_config --version
        /bin/sh: 1: mariadb_config: not found
        mysql_config --libs
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_d6fcfd51e48244b684a1f9a254001e48/setup.py", line 15, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_d6fcfd51e48244b684a1f9a254001e48/setup_posix.py", line 70, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_d6fcfd51e48244b684a1f9a254001e48/setup_posix.py", line 31, in mysql_config
            raise OSError("{} not found".format(_mysql_config_path))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/de/79/d02be3cb942afda6c99ca207858847572e38146eb73a7c4bfe3bdf154626/mysqlclient-2.1.0.tar.gz#sha256=973235686f1b720536d417bf0a0d39b4ab3d5086b2b6ad5e6752393428c02b12 (from https://pypi.org/simple/mysqlclient/) (requires-python:>=3.5). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-2.0.3.tar.gz (88 kB)
    [K     |████████████████████████████████| 88 kB 4.0 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_23175c1ca7b641e4a556a4d2b09bc015/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_23175c1ca7b641e4a556a4d2b09bc015/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-297hgf9t
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_23175c1ca7b641e4a556a4d2b09bc015/
        Complete output (15 lines):
        mysql_config --version
        /bin/sh: 1: mysql_config: not found
        mariadb_config --version
        /bin/sh: 1: mariadb_config: not found
        mysql_config --libs
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_23175c1ca7b641e4a556a4d2b09bc015/setup.py", line 15, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_23175c1ca7b641e4a556a4d2b09bc015/setup_posix.py", line 70, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_23175c1ca7b641e4a556a4d2b09bc015/setup_posix.py", line 31, in mysql_config
            raise OSError("{} not found".format(_mysql_config_path))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/3c/df/59cd2fa5e48d0804d213bdcb1acb4d08c403b61c7ff7ed4dd4a6a2deb3f7/mysqlclient-2.0.3.tar.gz#sha256=f6ebea7c008f155baeefe16c56cd3ee6239f7a5a9ae42396c2f1860f08a7c432 (from https://pypi.org/simple/mysqlclient/) (requires-python:>=3.5). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-2.0.2.tar.gz (88 kB)
    [K     |████████████████████████████████| 88 kB 3.8 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_53c8228b249e47f9aaffb151f4d16a0d/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_53c8228b249e47f9aaffb151f4d16a0d/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-6lvh5gep
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_53c8228b249e47f9aaffb151f4d16a0d/
        Complete output (12 lines):
        /bin/sh: 1: mysql_config: not found
        /bin/sh: 1: mariadb_config: not found
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_53c8228b249e47f9aaffb151f4d16a0d/setup.py", line 15, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_53c8228b249e47f9aaffb151f4d16a0d/setup_posix.py", line 65, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_53c8228b249e47f9aaffb151f4d16a0d/setup_posix.py", line 31, in mysql_config
            raise OSError("{} not found".format(_mysql_config_path))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/0e/68/f79de0e0fcdb041783124b825771e0ba6a3d0893b7b4c4735f130e42af47/mysqlclient-2.0.2.tar.gz#sha256=8df057b08fc27d8f7106bfa997d0a21e2acef017f905f06d6fb0aa6a20d4d2b2 (from https://pypi.org/simple/mysqlclient/) (requires-python:>=3.5). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-2.0.1.tar.gz (87 kB)
    [K     |████████████████████████████████| 87 kB 5.1 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_b221f1a6ba584cfbb10e86ada218398e/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_b221f1a6ba584cfbb10e86ada218398e/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-kxr_prqp
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_b221f1a6ba584cfbb10e86ada218398e/
        Complete output (12 lines):
        /bin/sh: 1: mysql_config: not found
        /bin/sh: 1: mariadb_config: not found
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_b221f1a6ba584cfbb10e86ada218398e/setup.py", line 15, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_b221f1a6ba584cfbb10e86ada218398e/setup_posix.py", line 65, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_b221f1a6ba584cfbb10e86ada218398e/setup_posix.py", line 31, in mysql_config
            raise OSError("{} not found".format(_mysql_config_path))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/a5/e1/e5f2b231c05dc51d9d87fa5066f90d1405345c54b14b0b11a1c859020f21/mysqlclient-2.0.1.tar.gz#sha256=fb2f75aea14722390d2d8ddf384ad99da708c707a96656210a7be8af20a2c5e5 (from https://pypi.org/simple/mysqlclient/) (requires-python:>=3.5). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-2.0.0.tar.gz (87 kB)
    [K     |████████████████████████████████| 87 kB 5.1 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_f5521c5391a841478ca7a16e2b263513/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_f5521c5391a841478ca7a16e2b263513/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-3fnuk05m
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_f5521c5391a841478ca7a16e2b263513/
        Complete output (12 lines):
        /bin/sh: 1: mysql_config: not found
        /bin/sh: 1: mariadb_config: not found
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_f5521c5391a841478ca7a16e2b263513/setup.py", line 15, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_f5521c5391a841478ca7a16e2b263513/setup_posix.py", line 65, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_f5521c5391a841478ca7a16e2b263513/setup_posix.py", line 31, in mysql_config
            raise OSError("{} not found".format(_mysql_config_path))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/ca/cf/dd8124bf8b3d2ae465db9c8ce35c51650c31784b095f41faf6f8cad987a0/mysqlclient-2.0.0.tar.gz#sha256=201dfcc2a3c8a0859ea399947f1af8abe74b706beba0ebac149180d9d7b0f6e8 (from https://pypi.org/simple/mysqlclient/) (requires-python:>=3.5). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.4.6.tar.gz (85 kB)
    [K     |████████████████████████████████| 85 kB 4.4 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_6fa8a9e6b9b24199a8da0a8d50730641/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_6fa8a9e6b9b24199a8da0a8d50730641/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-6dnpfr18
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_6fa8a9e6b9b24199a8da0a8d50730641/
        Complete output (12 lines):
        /bin/sh: 1: mysql_config: not found
        /bin/sh: 1: mariadb_config: not found
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_6fa8a9e6b9b24199a8da0a8d50730641/setup.py", line 16, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_6fa8a9e6b9b24199a8da0a8d50730641/setup_posix.py", line 61, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_6fa8a9e6b9b24199a8da0a8d50730641/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (_mysql_config_path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/d0/97/7326248ac8d5049968bf4ec708a5d3d4806e412a42e74160d7f266a3e03a/mysqlclient-1.4.6.tar.gz#sha256=f3fdaa9a38752a3b214a6fe79d7cae3653731a53e577821f9187e67cbecb2e16 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.4.5.tar.gz (86 kB)
    [K     |████████████████████████████████| 86 kB 5.1 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_808e0c626ebb4c889198bff022f6114d/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_808e0c626ebb4c889198bff022f6114d/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-303vo4js
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_808e0c626ebb4c889198bff022f6114d/
        Complete output (12 lines):
        /bin/sh: 1: mysql_config: not found
        /bin/sh: 1: mariadb_config: not found
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_808e0c626ebb4c889198bff022f6114d/setup.py", line 16, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_808e0c626ebb4c889198bff022f6114d/setup_posix.py", line 61, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_808e0c626ebb4c889198bff022f6114d/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (_mysql_config_path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/f8/9b/5db9a03e2088a87c26e3e4d4c7f7e8f4c2dbae610f9521cdfac15755a795/mysqlclient-1.4.5.tar.gz#sha256=e80109b0ae8d952b900b31b623181532e5e89376d707dcbeb63f99e69cefe559 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.4.4.tar.gz (86 kB)
    [K     |████████████████████████████████| 86 kB 3.8 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_186092998dd542c3a63796c40b2755c7/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_186092998dd542c3a63796c40b2755c7/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-pcoe7joj
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_186092998dd542c3a63796c40b2755c7/
        Complete output (12 lines):
        /bin/sh: 1: mysql_config: not found
        /bin/sh: 1: mariadb_config: not found
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_186092998dd542c3a63796c40b2755c7/setup.py", line 16, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_186092998dd542c3a63796c40b2755c7/setup_posix.py", line 61, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_186092998dd542c3a63796c40b2755c7/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (_mysql_config_path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/4d/38/c5f8bac9c50f3042c8f05615f84206f77f03db79781db841898fde1bb284/mysqlclient-1.4.4.tar.gz#sha256=9c737cc55a5dc8dd3583a942d5a9b21be58d16f00f5fefca4e575e7d9682e98c (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.4.3.tar.gz (86 kB)
    [K     |████████████████████████████████| 86 kB 3.5 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_e28f538601cd4c7f9e57bfb2ba743cd9/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_e28f538601cd4c7f9e57bfb2ba743cd9/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-p94hh3ar
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_e28f538601cd4c7f9e57bfb2ba743cd9/
        Complete output (12 lines):
        /bin/sh: 1: mysql_config: not found
        /bin/sh: 1: mariadb_config: not found
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_e28f538601cd4c7f9e57bfb2ba743cd9/setup.py", line 16, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_e28f538601cd4c7f9e57bfb2ba743cd9/setup_posix.py", line 61, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_e28f538601cd4c7f9e57bfb2ba743cd9/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (_mysql_config_path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/13/37/6c941aabeb78464a538b7d43266bfae645993779e3ca3e12fe82b4590f52/mysqlclient-1.4.3.tar.gz#sha256=0d3eeb97534c9f42e9b65bd35c1a35fadc2f6d7ea5d9fdbda5339a569156344b (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.4.2.post1.tar.gz (85 kB)
    [K     |████████████████████████████████| 85 kB 2.3 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_a925e4aec23140739bff31b2463939d6/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_a925e4aec23140739bff31b2463939d6/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-mqbtkrpr
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_a925e4aec23140739bff31b2463939d6/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_a925e4aec23140739bff31b2463939d6/setup.py", line 16, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_a925e4aec23140739bff31b2463939d6/setup_posix.py", line 51, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_a925e4aec23140739bff31b2463939d6/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (_mysql_config_path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/f4/f1/3bb6f64ca7a429729413e6556b7ba5976df06019a5245a43d36032f1061e/mysqlclient-1.4.2.post1.tar.gz#sha256=f257d250f2675d0ef99bd318906f3cfc05cef4a2f385ea695ff32a3f04b9f9a7 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.4.2.tar.gz (85 kB)
    [K     |████████████████████████████████| 85 kB 3.3 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_12b3ee903a384d22907cdca9459c205d/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_12b3ee903a384d22907cdca9459c205d/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-qmgoi7lk
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_12b3ee903a384d22907cdca9459c205d/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_12b3ee903a384d22907cdca9459c205d/setup.py", line 16, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_12b3ee903a384d22907cdca9459c205d/setup_posix.py", line 51, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_12b3ee903a384d22907cdca9459c205d/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (_mysql_config_path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/73/79/67ddf24ac31b05d741f0ac87fa612c7a11bab1b39b8270ed7344d149f8af/mysqlclient-1.4.2.tar.gz#sha256=b95edaa41d6cc47deecabcdcbb5ab437ad9ae6d8955f5cf10d1847b37e66ef5e (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.4.1.tar.gz (85 kB)
    [K     |████████████████████████████████| 85 kB 4.6 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_eb127de047bb41cca4cf69de25a9e47f/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_eb127de047bb41cca4cf69de25a9e47f/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-6tkt4dfr
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_eb127de047bb41cca4cf69de25a9e47f/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_eb127de047bb41cca4cf69de25a9e47f/setup.py", line 16, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_eb127de047bb41cca4cf69de25a9e47f/setup_posix.py", line 51, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_eb127de047bb41cca4cf69de25a9e47f/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (_mysql_config_path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/de/d7/919042fb7ed78a89e21c4e43d5daed90d5df18ec183bae3de493a7d9e3ed/mysqlclient-1.4.1.tar.gz#sha256=a62220410e26ce2d2ff94dd0138c3ecfb91db634464a9afb4c8e6b50f0a67e00 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.4.0.tar.gz (85 kB)
    [K     |████████████████████████████████| 85 kB 3.1 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_7023b0a2521e4f4bb90ed5db846146c4/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_7023b0a2521e4f4bb90ed5db846146c4/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-9pb5kzdb
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_7023b0a2521e4f4bb90ed5db846146c4/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_7023b0a2521e4f4bb90ed5db846146c4/setup.py", line 16, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_7023b0a2521e4f4bb90ed5db846146c4/setup_posix.py", line 51, in get_config
            libs = mysql_config("libs")
          File "/tmp/pip-install-juftnpcq/mysqlclient_7023b0a2521e4f4bb90ed5db846146c4/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (_mysql_config_path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/05/73/fac741eef89b0257fb1807de80e96474f40d52739cdbc32c90c4a793e79d/mysqlclient-1.4.0.tar.gz#sha256=efeaacd04feea7d44fef2a5adf4df335b438458f8b89144307dc5a90025761a5 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.14.tar.gz (91 kB)
    [K     |████████████████████████████████| 91 kB 5.8 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_b5cfee2b305a42c893f49da97929e16f/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_b5cfee2b305a42c893f49da97929e16f/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-8o0rau7q
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_b5cfee2b305a42c893f49da97929e16f/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_b5cfee2b305a42c893f49da97929e16f/setup.py", line 16, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_b5cfee2b305a42c893f49da97929e16f/setup_posix.py", line 53, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_b5cfee2b305a42c893f49da97929e16f/setup_posix.py", line 28, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/f7/a2/1230ebbb4b91f42ad6b646e59eb8855559817ad5505d81c1ca2b5a216040/mysqlclient-1.3.14.tar.gz#sha256=3981ae9ce545901a36a8b7aed76ed02960a429f75dc53b7ad77fb2f9ab7cd56b (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.13.tar.gz (90 kB)
    [K     |████████████████████████████████| 90 kB 6.0 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_a92d8d76cb8e47a99cc9f4cdfc7b00c4/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_a92d8d76cb8e47a99cc9f4cdfc7b00c4/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-efj1oatn
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_a92d8d76cb8e47a99cc9f4cdfc7b00c4/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_a92d8d76cb8e47a99cc9f4cdfc7b00c4/setup.py", line 18, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_a92d8d76cb8e47a99cc9f4cdfc7b00c4/setup_posix.py", line 53, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_a92d8d76cb8e47a99cc9f4cdfc7b00c4/setup_posix.py", line 28, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/ec/fd/83329b9d3e14f7344d1cb31f128e6dbba70c5975c9e57896815dbb1988ad/mysqlclient-1.3.13.tar.gz#sha256=ff8ee1be84215e6c30a746b728c41eb0701a46ca76e343af445b35ce6250644f (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.12.tar.gz (89 kB)
    [K     |████████████████████████████████| 89 kB 4.1 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_593e5d4df18740758c1dd74cb774a802/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_593e5d4df18740758c1dd74cb774a802/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-1okfaarf
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_593e5d4df18740758c1dd74cb774a802/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_593e5d4df18740758c1dd74cb774a802/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_593e5d4df18740758c1dd74cb774a802/setup_posix.py", line 44, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_593e5d4df18740758c1dd74cb774a802/setup_posix.py", line 26, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/6f/86/bad31f1c1bb0cc99e88ca2adb7cb5c71f7a6540c1bb001480513de76a931/mysqlclient-1.3.12.tar.gz#sha256=2d9ec33de39f4d9c64ad7322ede0521d85829ce36a76f9dd3d6ab76a9c8648e5 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.11.tar.gz (89 kB)
    [K     |████████████████████████████████| 89 kB 5.7 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_c0ff41cef88b4523aa2607d706b8a63f/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_c0ff41cef88b4523aa2607d706b8a63f/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-7k53z7c6
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_c0ff41cef88b4523aa2607d706b8a63f/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_c0ff41cef88b4523aa2607d706b8a63f/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_c0ff41cef88b4523aa2607d706b8a63f/setup_posix.py", line 44, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_c0ff41cef88b4523aa2607d706b8a63f/setup_posix.py", line 26, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/6a/4d/856d1848e9b7fa8577a31c0188592f472e5cbc94f588c2a40ff930533d73/mysqlclient-1.3.11.tar.gz#sha256=9a79b38843d61f651266ff16b9fdcc8830d21f0fb852e4406a19e9a715bdf3e2 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.10.tar.gz (82 kB)
    [K     |████████████████████████████████| 82 kB 496 kB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_ffd1afee71114d199c81d1616a3501f5/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_ffd1afee71114d199c81d1616a3501f5/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-3har43dc
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_ffd1afee71114d199c81d1616a3501f5/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_ffd1afee71114d199c81d1616a3501f5/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_ffd1afee71114d199c81d1616a3501f5/setup_posix.py", line 44, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_ffd1afee71114d199c81d1616a3501f5/setup_posix.py", line 26, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/40/9b/0bc869f290b8f49a99b8d97927f57126a5d1befcf8bac92c60dc855f2523/mysqlclient-1.3.10.tar.gz#sha256=452aaf9d2ba1a4fb85c134c88f9b1857852deed63b3b13255d7a65d2c1297262 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.9.tar.gz (81 kB)
    [K     |████████████████████████████████| 81 kB 4.5 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_a703c481f52043e78a77c31806f183e9/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_a703c481f52043e78a77c31806f183e9/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-rvgi3zq3
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_a703c481f52043e78a77c31806f183e9/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_a703c481f52043e78a77c31806f183e9/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_a703c481f52043e78a77c31806f183e9/setup_posix.py", line 44, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_a703c481f52043e78a77c31806f183e9/setup_posix.py", line 26, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/db/f5/c8e1657985c31dda16e434edf5257c31572fa5faacd7e48b1618390e4b18/mysqlclient-1.3.9.tar.gz#sha256=990ccf1e1f15b9a291b811c993dc1c216566714bc14e6581b38665bd61c28c99 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.8.tar.gz (81 kB)
    [K     |████████████████████████████████| 81 kB 5.4 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_dc81dfc1c212423eac031eb81273a247/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_dc81dfc1c212423eac031eb81273a247/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-9i19_ppq
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_dc81dfc1c212423eac031eb81273a247/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_dc81dfc1c212423eac031eb81273a247/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_dc81dfc1c212423eac031eb81273a247/setup_posix.py", line 44, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_dc81dfc1c212423eac031eb81273a247/setup_posix.py", line 26, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/31/ce/7ea049b3d5929b3cce3104967ccca218a9f054517f0d15dfdaf4e76da2a0/mysqlclient-1.3.8.tar.gz#sha256=c64bc386c0b771ed6ff76de0f52e0f957f98d9e13c83b0ddb821afdbe3f5d970 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.7.tar.gz (79 kB)
    [K     |████████████████████████████████| 79 kB 3.6 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_ebf0c09e0c304d1aaab4497c768ffe25/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_ebf0c09e0c304d1aaab4497c768ffe25/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-dhv_7wsc
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_ebf0c09e0c304d1aaab4497c768ffe25/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_ebf0c09e0c304d1aaab4497c768ffe25/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_ebf0c09e0c304d1aaab4497c768ffe25/setup_posix.py", line 44, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_ebf0c09e0c304d1aaab4497c768ffe25/setup_posix.py", line 26, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/74/ff/4e964e20b559e55d7afa60fbccc6a560f2adf289813bd3d7eb4eb8a87093/mysqlclient-1.3.7.tar.gz#sha256=c74a83b4cb2933d0e43370117eeebdfa03077ae72686d2df43d31879267f1f1b (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.6.tar.gz (78 kB)
    [K     |████████████████████████████████| 78 kB 4.2 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_df99df4f32cb45adab9be4a3b6f1debe/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_df99df4f32cb45adab9be4a3b6f1debe/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-a6s5zrb_
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_df99df4f32cb45adab9be4a3b6f1debe/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_df99df4f32cb45adab9be4a3b6f1debe/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_df99df4f32cb45adab9be4a3b6f1debe/setup_posix.py", line 47, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_df99df4f32cb45adab9be4a3b6f1debe/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/09/29/6648563af4b45798ba667f17ea55166d7b0ed8717937c06977a1fdbe7df6/mysqlclient-1.3.6.tar.gz#sha256=1f63a8ab111530a0ff9acaeb118074f11e7564b7c124f2e7fc56fcac641aecf2 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.5.tar.gz (77 kB)
    [K     |████████████████████████████████| 77 kB 3.7 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_83ef1e4995ba4c61970a0accce116f4c/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_83ef1e4995ba4c61970a0accce116f4c/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-k7x4z3yg
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_83ef1e4995ba4c61970a0accce116f4c/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_83ef1e4995ba4c61970a0accce116f4c/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_83ef1e4995ba4c61970a0accce116f4c/setup_posix.py", line 47, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_83ef1e4995ba4c61970a0accce116f4c/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/82/ea/336daf6c7baa564d0c434ab748218d1a7dc61dfc7066e98b72afd24fd2b9/mysqlclient-1.3.5.tar.gz#sha256=80ea68f6f3c2cfbf35c91adde2b40de1f2c31132118d2dcee048c72423f678bf (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.4.tar.gz (77 kB)
    [K     |████████████████████████████████| 77 kB 4.9 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_b0e6397c92de466a8074ba79b705daf2/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_b0e6397c92de466a8074ba79b705daf2/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-keqhuynt
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_b0e6397c92de466a8074ba79b705daf2/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_b0e6397c92de466a8074ba79b705daf2/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_b0e6397c92de466a8074ba79b705daf2/setup_posix.py", line 47, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_b0e6397c92de466a8074ba79b705daf2/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/17/d9/03b08e6a033401335b720806b87596aee8d7f7aa87539713238905c4a8d1/mysqlclient-1.3.4.tar.gz#sha256=a0263383f8ac33ad12d68dc61fa8ccbee41244ce916287c6cee71bf8aea82c5c (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.3.tar.gz (77 kB)
    [K     |████████████████████████████████| 77 kB 4.3 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_2a1ab668bf904f628cd11d4a0d891114/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_2a1ab668bf904f628cd11d4a0d891114/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-tw_wa4f7
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_2a1ab668bf904f628cd11d4a0d891114/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_2a1ab668bf904f628cd11d4a0d891114/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_2a1ab668bf904f628cd11d4a0d891114/setup_posix.py", line 47, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_2a1ab668bf904f628cd11d4a0d891114/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/26/53/c575db342bfca0213c9243ed2642bfadcd420b18d2f477dc812543e3d83a/mysqlclient-1.3.3.tar.gz#sha256=0f0887882d71bf2a079d9724d9323053cfbee8ab2dcfc989daf97d7ce5be9af9 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.2.tar.gz (77 kB)
    [K     |████████████████████████████████| 77 kB 4.0 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_709701e1cd414ee1b2c14efc0bf13231/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_709701e1cd414ee1b2c14efc0bf13231/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-_q0cqbce
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_709701e1cd414ee1b2c14efc0bf13231/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_709701e1cd414ee1b2c14efc0bf13231/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_709701e1cd414ee1b2c14efc0bf13231/setup_posix.py", line 47, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_709701e1cd414ee1b2c14efc0bf13231/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/2d/df/5440ee86bbb248325cdd6e1fc9cbbba365018a0d2d57f673610e020e6b1d/mysqlclient-1.3.2.tar.gz#sha256=e44025830501b9f70f8c2fe8eeff66f0df2df198802f7295801dac199b8236ef (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.1.tar.gz (76 kB)
    [K     |████████████████████████████████| 76 kB 3.6 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_c2cfc7f38cba402281a92abe2dffb068/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_c2cfc7f38cba402281a92abe2dffb068/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-hcw8_8i9
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_c2cfc7f38cba402281a92abe2dffb068/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_c2cfc7f38cba402281a92abe2dffb068/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_c2cfc7f38cba402281a92abe2dffb068/setup_posix.py", line 47, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_c2cfc7f38cba402281a92abe2dffb068/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/6b/ba/4729d99e85a0a35bb46d55500570de05b4af10431cef174b6da9f58a0e50/mysqlclient-1.3.1.tar.gz#sha256=3549e8a61f10c8cd8eac6581d3f44d0594f535fb7b29e6090db3a0bc547b25ad (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
      Downloading mysqlclient-1.3.0.tar.gz (76 kB)
    [K     |████████████████████████████████| 76 kB 4.8 MB/s eta 0:00:01
    [?25h[31m    ERROR: Command errored out with exit status 1:
         command: /home/moses/miniconda3/bin/python -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'/tmp/pip-install-juftnpcq/mysqlclient_34b890bdb1654ec7be45f876efde3a86/setup.py'"'"'; __file__='"'"'/tmp/pip-install-juftnpcq/mysqlclient_34b890bdb1654ec7be45f876efde3a86/setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' egg_info --egg-base /tmp/pip-pip-egg-info-iv84mxad
             cwd: /tmp/pip-install-juftnpcq/mysqlclient_34b890bdb1654ec7be45f876efde3a86/
        Complete output (10 lines):
        /bin/sh: 1: mysql_config: not found
        Traceback (most recent call last):
          File "<string>", line 1, in <module>
          File "/tmp/pip-install-juftnpcq/mysqlclient_34b890bdb1654ec7be45f876efde3a86/setup.py", line 17, in <module>
            metadata, options = get_config()
          File "/tmp/pip-install-juftnpcq/mysqlclient_34b890bdb1654ec7be45f876efde3a86/setup_posix.py", line 47, in get_config
            libs = mysql_config("libs_r")
          File "/tmp/pip-install-juftnpcq/mysqlclient_34b890bdb1654ec7be45f876efde3a86/setup_posix.py", line 29, in mysql_config
            raise EnvironmentError("%s not found" % (mysql_config.path,))
        OSError: mysql_config not found
        ----------------------------------------[0m
    [33mWARNING: Discarding https://files.pythonhosted.org/packages/6a/91/bdfe808fb5dc99a5f65833b370818161b77ef6d1e19b488e4c146ab615aa/mysqlclient-1.3.0.tar.gz#sha256=06eb5664e3738b283ea2262ee60ed83192e898f019cc7ff251f4d05a564ab3b7 (from https://pypi.org/simple/mysqlclient/). Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.[0m
    [31mERROR: Could not find a version that satisfies the requirement mysqlclient (from versions: 1.3.0, 1.3.1, 1.3.2, 1.3.3, 1.3.4, 1.3.5, 1.3.6, 1.3.7, 1.3.8, 1.3.9, 1.3.10, 1.3.11rc1, 1.3.11, 1.3.12, 1.3.13, 1.3.14, 1.4.0rc1, 1.4.0rc2, 1.4.0rc3, 1.4.0, 1.4.1, 1.4.2, 1.4.2.post1, 1.4.3, 1.4.4, 1.4.5, 1.4.6, 2.0.0, 2.0.1, 2.0.2, 2.0.3, 2.1.0rc1, 2.1.0, 2.1.1)[0m
    [31mERROR: No matching distribution found for mysqlclient[0m

