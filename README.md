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
    <td>summary(df)</td>
    <td>..</td>
    <td>..</td>
    <td>data.describe()</td>
  </tr>
  <tr>
    <td>display n-first observations</td>
    <td>head(df)</td>
    <td>..</td>
    <td>..</td>
    <td>df.head()</td>
  </tr>
  <tr>
    <td>display column's names</td>
    <td>names(df)</td>
    <td>..</td>
    <td>..</td>
    <td>df.columns</td>
  </tr>
  <tr>
    <td>slicing p first rows and q first cols</td>
    <td>df[1:p,1:q]</td>
    <td>..</td>
    <td>..</td>
    <td>df.iloc[:(p-1),:(q-1)]</td>
  </tr>
  <tr>
    <td>Selecting all obs. on a multi-axis by label</td>
    <td>df[,c('x','y')]</td>
    <td>dt[,list(x,y)]</td>
    <td>select(df,x,y)</td>
    <td>df.loc[:,['x,'y']]</td>
  </tr>
  <tr>
    <td>Using a single column’s value to select data</td>
    <td>df[df$x==value,]</td>
    <td>setkeyv(dt,x) ; dt[J(value),]</td>
    <td>df %>% select(df,x) %>% filter(df,x==value)</td>
    <td>df[df.x==value]</td>
  </tr>
</table> 


Feel free to contribute:
* by adding your favorite R or python commands even showing more complex tasks on both languages
* Reproducible examples such as ipython notebooks or Rpubs are also welcome.
