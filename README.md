# Week_14_Challenge
The purpose of this analysis is the creation and optimization of trading algorithims. 


---

## Technologies

This application is written in the python 3.7 language. It uses the 'pandas', 'pathlib', 'sklearn', 'hvplot' and 'numpy' libraries and dependencies. It has been developed and tested on MacOS


---
`
## Optimization

![](https://user-images.githubusercontent.com/106558893/190239966-1d3a8104-efac-444b-b50c-57faa3abc605.png)

This is the original strategy actual return vs strategy return. 

1. Change the size of the training dataset
    - The size of the training dataset was changed from the data start date until 6 months after. This was increased from the original 3 months of data. Increasing the training window to 6 months changes the strategy returns pretty significantly. The period from roughly 2019-2020 has a strategy return lower than the actual returns. Then after 2020 the strategy returns are higher than the actual returns. After 2020 the strategy returns are greater in this model than the original model. Below is a visualization of the new strategy.

    ![](https://user-images.githubusercontent.com/106558893/190239643-99a7c8b7-d064-4981-b0bd-2b8b363a672a.png)

2. Adjusting the SMA features
    - The SMA windows were changed to 2 and 25 for the small and large windows respectively. This caused the trading strategy to have a lower value than the actual returns from late 2017 until the end of the simulation. Below is a graph of the strategy's returns with adjusted SMA values.

    ![](https://user-images.githubusercontent.com/106558893/190239926-e2cf5a2f-e8b1-4f8b-864f-daf27a24b793.png)

3. Three models have been evaluated. Adjusting the SMA windows to 2 and 25 made the strategy return constantly below actual returns so that would not be a viable model. In terms of what is a better model that is subjective. The model with a 6 month training data window has higher cumulative returns at the end of the evaluation period than the original model. It also has lower strategy returns than the original model and actual returns for approximately a year. It depends on what the client using the model values in terms of risk vs reward. The 6 month training data window model has the highest potential reward, but also a lot more risk. If the risk is worth the reward will depend on what the model will be used for exactly and the user's temperance for risk. Charts of both models can be seen below. 

    ![](https://user-images.githubusercontent.com/106558893/190239976-f77840b9-6876-4697-a149-a583a35cfc42.png)
    ![](https://user-images.githubusercontent.com/106558893/190239643-99a7c8b7-d064-4981-b0bd-2b8b363a672a.png)


---
`
## Contributors

This application was developed by Jake Wheeler. I can be contacted at jpwheeler93@gmail.com


---

## License

MIT
