# Pricing Floating Rate Notes 

A floating rate note has variable coupons, depending on a money market reference rate, such as LIBOR, plus a floating spread. When interest rate raises, the coupons of an FRN increases in line with the increase of the forward rates, which means its price remains relatively constant. Therefore, FRNs bear small interest rate risk. On the other hand, FRNs carry lower yields than fixed rate bonds of the same maturity. They also have unpredictable coupon payments. 
The price of an FRN has very low sensitivity to changes in interest rates because the floating coupon increases but the discounting also increases as interest rate rises. An investor who wants conservative investments may choose floating rate bonds. FRNs become more popular when interest rates are expected to increase. An FRN carry lower yield than fixed rate bonds of the same maturity and has unpredictable coupon payments. This presentation gives an overview of FRNs valuation. 

	Floating Rate Note Introduction
	A floating rate note (FRN) is a bond in which the investor will receive coupons paid by the issuer at a floating coupon equivalent to a money market reference rate, such as LIBOR or federal fund rate plus a spread at specified dates before bond maturity.
	The bond principal will be returned at maturity date.
	Almost all FRNs have quarterly coupons.
	FRNs are usually issued by corporations, federal agencies, municipalities and states/provinces to finance a variety of projects and activities. 

	The Use of Floating Rate Notes
	A FRN carry little interest rate risk as its duration is close to zero due to periodic reset.
	The price of a FRN has very low sensitivity to changes in interest rates because the floating coupon increases but the discounting also increases as interest rate rises.
	An investor who wants conservative investments may choose floating rate bonds. 
	FRNs become more popular when interest rates are expected to increase.
	A FRN carry lower yield than fixed rate bonds of the same maturity.
	FRNs have unpredictable coupon payments.

	Valuation
	The present value of a FRN is given by
V(t)=∑_(i=1)^n▒〖F_i τ_i Pe^(-(r_i+s) T_i )+Pe^(-(r_n+s) T_n ) 〗
where
	t – valuation date
i – ith cash flow from 1 to n
	r_i – continuous compounded interest rate for the period (t,T_i)
T_i – coupon payment date of the ith  cash flow
s – credit spread
P – principal amount or face value
	   τ_i=τ(T_(i-1),T_i) – accrual period (T_(i-1),T_i) of the ith cash flow.
	   F_i=F(t;T_(i-1),T_i )=(D_(i-1)/D_i -1)/τ_i-  simply compounded forward rate
	   	D_i=D(t,T_i) –  discount factor

	Practical Guide
	The present value of a bond computed by any pricing models is the dirty price of the bond. To purchase a bond, the buyer pays this dirty price.
	Although investors pay dirty prices, bonds are typically quoted in terms of clean prices. 
Dirty Price = Clean Price + Accrued Interest
	The Yield-To-Maturity Model is a good tool to compute the present value or the fair value of a bond. But it is very difficult to calculate risk, such as term structure sensitivities, that is more important than the fair value in trading, hedging and risk management. Therefore, we introduce the Credit Spread Model for computing both risk and fair value.
	Intuitively,   e^(-(r+s)T)   can be regarded as a credit risk adjusted discount factor.
	To use the model, one should first calibrate the model price to the market quoted price by solving the credit spread. Comparing to curve construction or calibration for exotic products, the solving here is very simple.
	After making the model price equal to the market price, one can calculate sensitivities by shocking interest rate curve and credit spread.
	We use LIBOR curve plus credit spread rather than bond specific curves for discounting because bond specific curves rarely exist in the market, especially issued by small entities. Using LIBOR curve plus credit spread not only accounts for credit/issuer risk but also solves the missing data issue.
	Usually the forecasting curve is different from the discounting curve. For instance, the forecasting curve is the treasury curve but the discounting curve is the LIBOR curve plus credit spread.

 
	A Real World Example
Buy Sell	Buy
Calendar	NYC
Coupon Type	Floating
Currency	USD
First Coupon Date	10/31/2015
Interest Accrual Date	7/31/2015
Issue Date	7/31/2015
Last Coupon Date	4/30/2017
Maturity Date	7/31/2017
Settlement Date	7/31/2015
Settlement Lag	1
Notional	100
Pay Receive	Receive
Day Count	dcAct360
Payment Frequency	3M
Spread	0.00077


You can find more details at
https://finpricing.com/lib/IrCurveIntroduction.html
