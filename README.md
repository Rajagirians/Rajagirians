print('Hello, master, I'm your financial manager, xiaozhaocai')
print('Now let me do a family financial health diagnosis for you')
print('----------step 1------------------')
cash = float(input('Please tell xiaozhaocai the amount of cash and cash equivalent at home:'))
monthly_costs = float(input('Please tell us about the monthly expenditure of the company:')) 
# Liquidity ratio = cash, monthly expenditure
liquidity_ratio = cash/monthly_costs
print('The liquidity ratio has been calculated:',liquidity_ratio)
if 3<liquidity_ratio<6:
    print('Liquidity ratio in a reasonable range, this indicator shows the ability to deal with emergencies')
print('----------step 2------------------')
total_asset = float(input('Please tell xiaozhaocai the total assets of the family:'))
total_liability = float(input('Please tell xiaozhaocai the total family debt:'))
asset_liability_ratio = total_liability/total_asset
print('Asset liability ratio has been calculated:',asset_liability_ratio)
if asset_liability_ratio < 0.5:
    print('The asset liability ratio is less than 50%%，Debt health')
# Asset liability ratio = Total Liabilities / total assets
print('----------step 3------------------')
monthly_repayment_amount = float(input('Please tell xiaozhaocai the monthly repayment amount:'))
monthly_income = float(input('Please tell Xiao Zhaocai's monthly income:'))
Debt_service_ratio = monthly_repayment_amount/monthly_income
print('The debt repayment rate has been calculated:',Debt_service_ratio)
if Debt_service_ratio < 0.5:
    print('Debt repayment rate<50%，Qualified, this indicator tests debt repayment ability, and banks use it to measure the resilience of household funds when reviewing loans.')
# Debt repayment rate = monthly repayment amount / monthly income
print('----------step 4------------------')
monthly_savings = float(input('Please tell xiaozhaocai about his monthly savings:'))
savings_ratio = monthly_savings/monthly_income
print('The savings ratio has been calculated:',savings_ratio)
if savings_ratio>0.3:
    print('The saving ratio is greater than 30%，The higher the ratio, the faster the accumulation of wealth')
# Saving ratio = monthly savings / monthly income
print('----------step 5------------------')
investment_amount = float(input('Please tell us the amount of investment funds and stocks in the family of little Zhaocai:'))
net_asset = total_asset - total_liability
investment_ratio = investment_amount/net_asset
# Investment rate = investment amount / net assets
print('The investment rate has been calculated:',investment_ratio )
if investment_ratio>0.5:
    print('Investment rate>50%，The higher the proportion, the stronger the ability of wealth appreciation')
print('----------------------------------')
