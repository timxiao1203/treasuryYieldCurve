# Treasury Yield Curve Introduction

Treasury yield curve or treasury zero coupon yield curve is the term structures of treasury yields-to-maturity. The yield is also called the zero coupon rate or the implied forward rate.

Treasury yield curves are bootstrapped from treasury benchmark curves that contain the most actively traded treasury bills or bonds at some maturities.

There are four elements in interest rate: zero coupon rates (or zero rates), discount factor, par yields, and forward rates. The derivation of one of these element is conveniently sufficient for the determination of the other three elements. Each interest rate definition is derived from specific representations of bond price.

The zero coupon rate or zero rate, the most common form of interest rate, is the yield implied by the different between a zero coupon bond's current purchase price and the value it pays at maturity. A given zero rate applies only to a single point in the future and, as such, can only be used to discount cash flows occurring on this date. Zero rates can have different compoundings: continuously, semi-annually, annually, etc. The continuously compounded zero rate has the simplest expression and computation mathematically.

The discount factor for a corresponding term to maturity is equal to exp(-Z*T), where Z is the continuously compounded zero rate from 0 to T and T is the maturity date. The calculation of zero rates and their associated discount factors is essential for asset pricing.

Unfortunately both zero rates and discount factors prevailing in the market are not observable for all maturities. FinPricing bootstraps treasury benchmark curves to generate treasury yield curves (or treasury zero rate curves). All the yield curves generated by FinPricing are continuously compounded.


Treasury Yield Curve Data Sample

A treasury yield curve is shown below:

CurveName	ValuationDate	Tenor	Value
CAD_Treasury	2020-11-25	3/4/2021  	0.0010898
CAD_Treasury	2020-11-25	5/13/2021 	0.0015195
CAD_Treasury	2020-11-25	11/10/2021	0.002038
CAD_Treasury	2020-11-25	11/1/2022 	0.0026914
CAD_Treasury	2020-11-25	9/1/2023  	0.0030583
CAD_Treasury	2020-11-25	9/1/2024  	0.0036062
CAD_Treasury	2020-11-25	9/1/2025  	0.0045096
CAD_Treasury	2020-11-25	6/1/2026  	0.0046731
CAD_Treasury	2020-11-25	6/1/2027  	0.0051644
CAD_Treasury	2020-11-25	6/1/2028  	0.0058674
CAD_Treasury	2020-11-25	6/1/2029  	0.0064962
CAD_Treasury	2020-11-25	6/1/2030  	0.0071914
CAD_Treasury	2020-11-25	6/1/2041  	0.0113203
CAD_Treasury	2020-11-25	12/1/2051 	0.0127914

References:

https://finpricing.com/lib/IrBasisCurve.html

