Git location: https://gitlab.com/TheInceptors/finmark/CodeLibrary.git

#### Import csv as panda dataframe
* dailyFullUsdChfD1_pd = pd.read_csv('datasets/2018-05-02-UsdChfD1.csv')

#### Renaming panda dataframe columns
* dailyFullUsdChfD1_pd.columns = ['0', '0','DHigh','DLow','0', '0']

#### Picking a column argument dataframe 
* mDataTime0400_pd = hourlyFullUsdChf_pd [(hourlyFullUsdChf_pd['Time'] == '04:00')]

#### Numpy count results
* (BuyPosSubResult_np == 'Success').sum()

#### Python 3 length count
* countResultForSell = len(SellPosSubResult_np)

#### Drop NaN
* df.dropna()
* https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.dropna.html

#### Slicing columns 
* H1_UsdChf_Reshaped01_pd = H1_UsdChf_pd.drop(H1_UsdChf_pd.columns[[0, -1]], axis=1)
