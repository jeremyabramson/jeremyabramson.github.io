```python
import pandas as pd
```


```python
df = pd.read_csv('/Users/abramson/Desktop/cfb_data/2017/CSV/PBP - 2017 - Week 1.csv')
```


```python
df[(df.homeTeam == 'Miami') & (df.isScoringPlay == True)]
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
      <th>gameId</th>
      <th>year</th>
      <th>week</th>
      <th>homeId</th>
      <th>homeTeam</th>
      <th>homeAbbr</th>
      <th>awayId</th>
      <th>awayTeam</th>
      <th>awayAbbr</th>
      <th>driveIndex</th>
      <th>...</th>
      <th>isScoringPlay</th>
      <th>quarter</th>
      <th>clock</th>
      <th>type</th>
      <th>down</th>
      <th>distance</th>
      <th>yardLine</th>
      <th>yardsGained</th>
      <th>endYardLine</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>7032</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>0</td>
      <td>...</td>
      <td>True</td>
      <td>1</td>
      <td>7:25</td>
      <td>Field Goal Good</td>
      <td>4</td>
      <td>16</td>
      <td>19</td>
      <td>36</td>
      <td>19</td>
      <td>Uriel Hernandez 36 yd FG GOOD</td>
    </tr>
    <tr>
      <td>7045</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>1</td>
      <td>...</td>
      <td>True</td>
      <td>1</td>
      <td>3:19</td>
      <td>Field Goal Good</td>
      <td>4</td>
      <td>0</td>
      <td>90</td>
      <td>27</td>
      <td>90</td>
      <td>Michael Badgley 27 yd FG GOOD</td>
    </tr>
    <tr>
      <td>7064</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>3</td>
      <td>...</td>
      <td>True</td>
      <td>2</td>
      <td>13:31</td>
      <td>Rushing Touchdown</td>
      <td>1</td>
      <td>0</td>
      <td>95</td>
      <td>5</td>
      <td>100</td>
      <td>Mark Walton run for 5 yds for a TD, (Michael B...</td>
    </tr>
    <tr>
      <td>7078</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>5</td>
      <td>...</td>
      <td>True</td>
      <td>2</td>
      <td>8:31</td>
      <td>Passing Touchdown</td>
      <td>3</td>
      <td>0</td>
      <td>95</td>
      <td>5</td>
      <td>100</td>
      <td>Malik Rosier pass complete to Lawrence Cager f...</td>
    </tr>
    <tr>
      <td>7087</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>7</td>
      <td>...</td>
      <td>True</td>
      <td>2</td>
      <td>5:34</td>
      <td>Passing Touchdown</td>
      <td>2</td>
      <td>4</td>
      <td>95</td>
      <td>5</td>
      <td>100</td>
      <td>Malik Rosier pass complete to Darrell Langham ...</td>
    </tr>
    <tr>
      <td>7105</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>8</td>
      <td>...</td>
      <td>True</td>
      <td>2</td>
      <td>0:53</td>
      <td>Field Goal Good</td>
      <td>4</td>
      <td>0</td>
      <td>18</td>
      <td>35</td>
      <td>18</td>
      <td>Uriel Hernandez 35 yd FG GOOD</td>
    </tr>
    <tr>
      <td>7122</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>10</td>
      <td>...</td>
      <td>True</td>
      <td>3</td>
      <td>12:30</td>
      <td>Rushing Touchdown</td>
      <td>1</td>
      <td>0</td>
      <td>94</td>
      <td>6</td>
      <td>100</td>
      <td>Mark Walton run for 6 yds for a TD, (Michael B...</td>
    </tr>
    <tr>
      <td>7136</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>11</td>
      <td>...</td>
      <td>True</td>
      <td>3</td>
      <td>6:16</td>
      <td>Rushing Touchdown</td>
      <td>2</td>
      <td>0</td>
      <td>1</td>
      <td>1</td>
      <td>0</td>
      <td>Michael Jones run for 1 yd for a TD, (Uriel He...</td>
    </tr>
    <tr>
      <td>7155</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>14</td>
      <td>...</td>
      <td>True</td>
      <td>3</td>
      <td>1:08</td>
      <td>Passing Touchdown</td>
      <td>1</td>
      <td>10</td>
      <td>78</td>
      <td>22</td>
      <td>100</td>
      <td>Malik Rosier pass complete to Braxton Berrios ...</td>
    </tr>
    <tr>
      <td>7187</td>
      <td>400937449</td>
      <td>2017</td>
      <td>1</td>
      <td>2390</td>
      <td>Miami</td>
      <td>MIAMI</td>
      <td>2065</td>
      <td>Bethune-Cookman</td>
      <td>BCU</td>
      <td>18</td>
      <td>...</td>
      <td>True</td>
      <td>4</td>
      <td>5:14</td>
      <td>Field Goal Good</td>
      <td>4</td>
      <td>23</td>
      <td>67</td>
      <td>50</td>
      <td>80</td>
      <td>Michael Badgley 50 yd FG GOOD</td>
    </tr>
  </tbody>
</table>
<p>10 rows × 29 columns</p>
</div>




```python
df.columns
```




    Index(['gameId', 'year', 'week', 'homeId', 'homeTeam', 'homeAbbr', 'awayId',
           'awayTeam', 'awayAbbr', 'driveIndex', 'playIndex', 'offenseId',
           'offenseTeam', 'offenseAbbr', 'defenseId', 'defenseTeam', 'defenseAbbr',
           'homeScore', 'awayScore', 'isScoringPlay', 'quarter', 'clock', 'type',
           'down', 'distance', 'yardLine', 'yardsGained', 'endYardLine',
           'description'],
          dtype='object')




```python

```
