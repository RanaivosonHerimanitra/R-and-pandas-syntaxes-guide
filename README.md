R-and-pandas-syntaxes-guide
===========================

Similarities between R and pandas syntaxes to help beginners.

 <table style="width:100%">
  <tr>
    <td>Operations</td>
    <td>R</td>
    <td>R::data.table</td>
    <td>R::dplyr</td>
    <td>pandas</td>
  </tr>
  <tr>
    <td>Summarize a dataset</td>
    <td>summary(data)</td>
    <td>..</td>
    <td>..</td>
    <td>data.describe()</td>
  </tr>
  <tr>
    <td>display n-first observations</td>
    <td>head(data)</td>
    <td>..</td>
    <td>..</td>
    <td>data.head()</td>
  </tr>
  <tr>
    <td>display column's names</td>
    <td>names(data)</td>
    <td>..</td>
    <td>..</td>
    <td>data.columns</td>
  </tr>
  <tr>
    <td>slicing p first rows and q first cols</td>
    <td>data[1:p,1:q]</td>
    <td>..</td>
    <td>..</td>
    <td>data.iloc[:(p-1),:(q-1)]</td>
  </tr>
  <tr>
    <td>Selecting all obs. on a multi-axis by label (x,y are known in advance)</td>
    <td>data[,c('x','y')]</td>
    <td>..</td>
    <td>..</td>
    <td>data.loc[:,['x,'y']]</td>
  </tr>
</table> 


#### Feel free to contribute by adding your favorite R or python commands
