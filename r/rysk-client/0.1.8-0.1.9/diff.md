# Comparing `tmp/rysk_client-0.1.8.tar.gz` & `tmp/rysk_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rysk_client-0.1.8.tar", max compression
+gzip compressed data, was "rysk_client-0.1.9.tar", max compression
```

## Comparing `rysk_client-0.1.8.tar` & `rysk_client-0.1.9.tar`

### file list

```diff
@@ -1,315 +1,318 @@
--rw-r--r--   0        0        0    26677 2023-06-04 11:48:29.236208 rysk_client-0.1.8/README.md
--rw-r--r--   0        0        0      600 2023-06-04 11:48:29.240208 rysk_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/__init__.py
--rw-r--r--   0        0        0     2431 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/cli.py
--rw-r--r--   0        0        0    13272 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/client.py
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/contracts/Accounting.sol/Accounting.dbg.json
--rw-r--r--   0        0        0    32509 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/contracts/Accounting.sol/Accounting.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/contracts/AlphaOptionHandler.sol/AlphaOptionHandler.dbg.json
--rw-r--r--   0        0        0    55200 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/contracts/AlphaOptionHandler.sol/AlphaOptionHandler.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/contracts/AlphaPortfolioValuesFeed.sol/AlphaPortfolioValuesFeed.dbg.json
--rw-r--r--   0        0        0    58641 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/contracts/AlphaPortfolioValuesFeed.sol/AlphaPortfolioValuesFeed.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.240208 rysk_client-0.1.8/rysk_client/contracts/Authority.sol/Authority.dbg.json
--rw-r--r--   0        0        0    14683 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/Authority.sol/Authority.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/BeyondPricer.sol/BeyondPricer.dbg.json
--rw-r--r--   0        0        0    69533 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/BeyondPricer.sol/BeyondPricer.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/LiquidityPool.sol/LiquidityPool.dbg.json
--rw-r--r--   0        0        0   134569 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/LiquidityPool.sol/LiquidityPool.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/Manager.sol/Manager.dbg.json
--rw-r--r--   0        0        0    43720 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/Manager.sol/Manager.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/OptionCatalogue.sol/OptionCatalogue.dbg.json
--rw-r--r--   0        0        0    30256 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/OptionCatalogue.sol/OptionCatalogue.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/OptionExchange.sol/OptionExchange.dbg.json
--rw-r--r--   0        0        0   129629 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/OptionExchange.sol/OptionExchange.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/OptionRegistry.sol/OptionRegistry.dbg.json
--rw-r--r--   0        0        0   105395 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/OptionRegistry.sol/OptionRegistry.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/PriceFeed.sol/PriceFeed.dbg.json
--rw-r--r--   0        0        0    16525 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/PriceFeed.sol/PriceFeed.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.244208 rysk_client-0.1.8/rysk_client/contracts/Protocol.sol/Protocol.dbg.json
--rw-r--r--   0        0        0     9497 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/Protocol.sol/Protocol.json
--rw-r--r--   0        0        0      105 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/VolatilityFeed.sol/VolatilityFeed.dbg.json
--rw-r--r--   0        0        0    50343 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/VolatilityFeed.sol/VolatilityFeed.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/gelato/OpynPricerResolver.sol/OpynPricerResolver.dbg.json
--rw-r--r--   0        0        0     9140 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/gelato/OpynPricerResolver.sol/OpynPricerResolver.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/gelato/VaultCollateralMulticall.sol/VaultCollateralMulticall.dbg.json
--rw-r--r--   0        0        0     8662 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/gelato/VaultCollateralMulticall.sol/VaultCollateralMulticall.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/hedging/GmxHedgingReactor.sol/GmxHedgingReactor.dbg.json
--rw-r--r--   0        0        0    89973 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/hedging/GmxHedgingReactor.sol/GmxHedgingReactor.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/hedging/PerpHedgingReactor.sol/PerpHedgingReactor.dbg.json
--rw-r--r--   0        0        0    59661 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/hedging/PerpHedgingReactor.sol/PerpHedgingReactor.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/hedging/UniswapV3HedgingReactor.sol/UniswapV3HedgingReactor.dbg.json
--rw-r--r--   0        0        0    34523 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/hedging/UniswapV3HedgingReactor.sol/UniswapV3HedgingReactor.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.248208 rysk_client-0.1.8/rysk_client/contracts/hedging/UniswapV3RangeOrderReactor.sol/UniswapV3RangeOrderReactor.dbg.json
--rw-r--r--   0        0        0    91201 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/hedging/UniswapV3RangeOrderReactor.sol/UniswapV3RangeOrderReactor.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/AddressBookInterface.sol/AddressBookInterface.dbg.json
--rw-r--r--   0        0        0     5293 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/AddressBookInterface.sol/AddressBookInterface.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/AggregatorInterface.sol/AggregatorInterface.dbg.json
--rw-r--r--   0        0        0     5198 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/AggregatorInterface.sol/AggregatorInterface.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/AggregatorV3Interface.sol/AggregatorV3Interface.dbg.json
--rw-r--r--   0        0        0     2596 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/AggregatorV3Interface.sol/AggregatorV3Interface.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/GammaTypes.dbg.json
--rw-r--r--   0        0        0      699 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/GammaTypes.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/IController.dbg.json
--rw-r--r--   0        0        0     7300 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/IController.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/IOtoken.dbg.json
--rw-r--r--   0        0        0     1774 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/IOtoken.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/IOtokenFactory.dbg.json
--rw-r--r--   0        0        0     4447 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/IOtokenFactory.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAccounting.sol/IAccounting.dbg.json
--rw-r--r--   0        0        0     5466 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAccounting.sol/IAccounting.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAddressBook.sol/IAddressBook.dbg.json
--rw-r--r--   0        0        0      500 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAddressBook.sol/IAddressBook.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAlphaOptionHandler.sol/IAlphaOptionHandler.dbg.json
--rw-r--r--   0        0        0     5572 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAlphaOptionHandler.sol/IAlphaOptionHandler.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAlphaPortfolioValuesFeed.sol/IAlphaPortfolioValuesFeed.dbg.json
--rw-r--r--   0        0        0     6033 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAlphaPortfolioValuesFeed.sol/IAlphaPortfolioValuesFeed.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAuthority.sol/IAuthority.dbg.json
--rw-r--r--   0        0        0     3351 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IAuthority.sol/IAuthority.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IChainlinkPricer.sol/IChainlinkPricer.dbg.json
--rw-r--r--   0        0        0      657 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IChainlinkPricer.sol/IChainlinkPricer.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IGmxVault.sol/IGmxVault.dbg.json
--rw-r--r--   0        0        0    35992 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IGmxVault.sol/IGmxVault.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IGmxVaultPriceFeed.sol/IVaultPriceFeed.dbg.json
--rw-r--r--   0        0        0     6762 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IGmxVaultPriceFeed.sol/IVaultPriceFeed.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IHedgingReactor.sol/IHedgingReactor.dbg.json
--rw-r--r--   0        0        0     1789 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IHedgingReactor.sol/IHedgingReactor.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/ILiquidityPool.sol/ILiquidityPool.dbg.json
--rw-r--r--   0        0        0    21076 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/ILiquidityPool.sol/ILiquidityPool.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IMarginCalculator.sol/IMarginCalculator.dbg.json
--rw-r--r--   0        0        0     1610 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IMarginCalculator.sol/IMarginCalculator.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IOptionRegistry.sol/IOptionRegistry.dbg.json
--rw-r--r--   0        0        0     8964 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IOptionRegistry.sol/IOptionRegistry.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IOracle.sol/IOracle.dbg.json
--rw-r--r--   0        0        0     1714 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IOracle.sol/IOracle.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IPortfolioValuesFeed.sol/IPortfolioValuesFeed.dbg.json
--rw-r--r--   0        0        0     3777 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IPortfolioValuesFeed.sol/IPortfolioValuesFeed.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.252209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IPositionRouter.sol/IPositionRouter.dbg.json
--rw-r--r--   0        0        0     7286 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IPositionRouter.sol/IPositionRouter.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IPriceFeedTimelock.sol/IPriceFeedTimelock.dbg.json
--rw-r--r--   0        0        0     2430 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IPriceFeedTimelock.sol/IPriceFeedTimelock.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IReader.sol/IReader.dbg.json
--rw-r--r--   0        0        0     1099 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IReader.sol/IReader.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IRouter.sol/IRouter.dbg.json
--rw-r--r--   0        0        0     4125 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IRouter.sol/IRouter.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IWhitelist.sol/IWhitelist.dbg.json
--rw-r--r--   0        0        0     3225 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/IWhitelist.sol/IWhitelist.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/I_ERC20.sol/I_ERC20.dbg.json
--rw-r--r--   0        0        0     4001 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/I_ERC20.sol/I_ERC20.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/OtokenInterface.sol/OtokenInterface.dbg.json
--rw-r--r--   0        0        0     4570 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/OtokenInterface.sol/OtokenInterface.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/WETH.sol/WETH.dbg.json
--rw-r--r--   0        0        0     3229 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/interfaces/WETH.sol/WETH.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/lens/DHVLensMK1.sol/DHVLensMK1.dbg.json
--rw-r--r--   0        0        0    40159 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/lens/DHVLensMK1.sol/DHVLensMK1.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/AccessControl.sol/AccessControl.dbg.json
--rw-r--r--   0        0        0     1163 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/AccessControl.sol/AccessControl.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/BlackScholes.sol/BlackScholes.dbg.json
--rw-r--r--   0        0        0    37568 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/BlackScholes.sol/BlackScholes.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/CombinedActions.sol/CombinedActions.dbg.json
--rw-r--r--   0        0        0      704 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/CombinedActions.sol/CombinedActions.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/CustomErrors.sol/CustomErrors.dbg.json
--rw-r--r--   0        0        0     7217 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/CustomErrors.sol/CustomErrors.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/EnumerableSet.sol/EnumerableSet.dbg.json
--rw-r--r--   0        0        0      700 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/EnumerableSet.sol/EnumerableSet.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/NormalDist.sol/NormalDist.dbg.json
--rw-r--r--   0        0        0    18234 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/NormalDist.sol/NormalDist.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/OptionsCompute.sol/OptionsCompute.dbg.json
--rw-r--r--   0        0        0     9215 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/OptionsCompute.sol/OptionsCompute.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/OpynInteractions.sol/OpynInteractions.dbg.json
--rw-r--r--   0        0        0    33677 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/OpynInteractions.sol/OpynInteractions.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/RyskActions.sol/RyskActions.dbg.json
--rw-r--r--   0        0        0      696 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/RyskActions.sol/RyskActions.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/SABR.sol/SABR.dbg.json
--rw-r--r--   0        0        0      682 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/SABR.sol/SABR.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/SafeTransferLib.sol/SafeTransferLib.dbg.json
--rw-r--r--   0        0        0      704 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/SafeTransferLib.sol/SafeTransferLib.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/Types.sol/Types.dbg.json
--rw-r--r--   0        0        0      684 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/libraries/Types.sol/Types.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/mocks/ForceSend.sol/ForceSend.dbg.json
--rw-r--r--   0        0        0     1207 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/mocks/ForceSend.sol/ForceSend.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/mocks/MockChainlinkAggregator.sol/MockChainlinkAggregator.dbg.json
--rw-r--r--   0        0        0     6246 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/mocks/MockChainlinkAggregator.sol/MockChainlinkAggregator.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/mocks/MockChainlinkSequencerFeed.sol/MockChainlinkSequencerFeed.dbg.json
--rw-r--r--   0        0        0     2861 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/mocks/MockChainlinkSequencerFeed.sol/MockChainlinkSequencerFeed.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/mocks/MockPortfolioValuesFeed.sol/MockPortfolioValuesFeed.dbg.json
--rw-r--r--   0        0        0    23550 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/mocks/MockPortfolioValuesFeed.sol/MockPortfolioValuesFeed.json
--rw-r--r--   0        0        0      111 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/Migrations.sol/Migrations.dbg.json
--rw-r--r--   0        0        0     2244 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/Migrations.sol/Migrations.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.256209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/AddressBook.sol/AddressBook.dbg.json
--rw-r--r--   0        0        0    27786 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/AddressBook.sol/AddressBook.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Controller.sol/Controller.dbg.json
--rw-r--r--   0        0        0   127044 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Controller.sol/Controller.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/MarginCalculator.sol/MarginCalculator.dbg.json
--rw-r--r--   0        0        0    89218 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/MarginCalculator.sol/MarginCalculator.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/MarginPool.sol/MarginPool.dbg.json
--rw-r--r--   0        0        0    30610 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/MarginPool.sol/MarginPool.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Oracle.sol/Oracle.dbg.json
--rw-r--r--   0        0        0    36101 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Oracle.sol/Oracle.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Otoken.sol/Otoken.dbg.json
--rw-r--r--   0        0        0    60378 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Otoken.sol/Otoken.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/OtokenFactory.sol/OtokenFactory.dbg.json
--rw-r--r--   0        0        0    24205 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/OtokenFactory.sol/OtokenFactory.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/OtokenSpawner.sol/OtokenSpawner.dbg.json
--rw-r--r--   0        0        0      565 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/OtokenSpawner.sol/OtokenSpawner.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Whitelist.sol/Whitelist.dbg.json
--rw-r--r--   0        0        0    24760 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Whitelist.sol/Whitelist.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/external/callees/PermitCallee.sol/PermitCallee.dbg.json
--rw-r--r--   0        0        0     3477 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/external/callees/PermitCallee.sol/PermitCallee.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/external/canonical-weth/WETH9.sol/WETH9.dbg.json
--rw-r--r--   0        0        0    14660 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/external/canonical-weth/WETH9.sol/WETH9.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/external/proxies/PayableProxyController.sol/PayableProxyController.dbg.json
--rw-r--r--   0        0        0    21982 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/external/proxies/PayableProxyController.sol/PayableProxyController.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/AddressBookInterface.sol/AddressBookInterface.dbg.json
--rw-r--r--   0        0        0     5307 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/AddressBookInterface.sol/AddressBookInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/AggregatorInterface.sol/AggregatorInterface.dbg.json
--rw-r--r--   0        0        0     5212 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/AggregatorInterface.sol/AggregatorInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/CTokenInterface.sol/CTokenInterface.dbg.json
--rw-r--r--   0        0        0      781 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/CTokenInterface.sol/CTokenInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/CalleeInterface.sol/CalleeInterface.dbg.json
--rw-r--r--   0        0        0      653 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/CalleeInterface.sol/CalleeInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/ERC20Interface.sol/ERC20Interface.dbg.json
--rw-r--r--   0        0        0     4639 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/ERC20Interface.sol/ERC20Interface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/MarginCalculatorInterface.sol/MarginCalculatorInterface.dbg.json
--rw-r--r--   0        0        0     4342 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/MarginCalculatorInterface.sol/MarginCalculatorInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/MarginPoolInterface.sol/MarginPoolInterface.dbg.json
--rw-r--r--   0        0        0     3944 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/MarginPoolInterface.sol/MarginPoolInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/OpynPricerInterface.sol/OpynPricerInterface.dbg.json
--rw-r--r--   0        0        0     1017 2023-06-04 11:48:29.260209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/OpynPricerInterface.sol/OpynPricerInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/OracleInterface.sol/OracleInterface.dbg.json
--rw-r--r--   0        0        0     7103 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/OracleInterface.sol/OracleInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/OtokenInterface.sol/OtokenInterface.dbg.json
--rw-r--r--   0        0        0     4584 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/OtokenInterface.sol/OtokenInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/WETH9Interface.sol/WETH9Interface.dbg.json
--rw-r--r--   0        0        0     2475 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/WETH9Interface.sol/WETH9Interface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/WSTETHInterface.sol/WSTETHInterface.dbg.json
--rw-r--r--   0        0        0     1266 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/WSTETHInterface.sol/WSTETHInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/WhitelistInterface.sol/WhitelistInterface.dbg.json
--rw-r--r--   0        0        0     7545 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/WhitelistInterface.sol/WhitelistInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/YearnVaultInterface.sol/YearnVaultInterface.dbg.json
--rw-r--r--   0        0        0     1789 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/YearnVaultInterface.sol/YearnVaultInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/ZeroXExchangeInterface.sol/ZeroXExchangeInterface.dbg.json
--rw-r--r--   0        0        0     3503 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/ZeroXExchangeInterface.sol/ZeroXExchangeInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/Actions.sol/Actions.dbg.json
--rw-r--r--   0        0        0      657 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/Actions.sol/Actions.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/FixedPointInt256.sol/FixedPointInt256.dbg.json
--rw-r--r--   0        0        0      675 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/FixedPointInt256.sol/FixedPointInt256.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/MarginVault.sol/MarginVault.dbg.json
--rw-r--r--   0        0        0    11131 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/MarginVault.sol/MarginVault.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/SignedConverter.sol/SignedConverter.dbg.json
--rw-r--r--   0        0        0      673 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/SignedConverter.sol/SignedConverter.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewCalculator.sol/NewMarginCalculator.dbg.json
--rw-r--r--   0        0        0    94183 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewCalculator.sol/NewMarginCalculator.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewController.sol/NewController.dbg.json
--rw-r--r--   0        0        0   129863 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewController.sol/NewController.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewMarginCalculatorInterface.sol/MarginCalculatorInterface.dbg.json
--rw-r--r--   0        0        0     4096 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewMarginCalculatorInterface.sol/MarginCalculatorInterface.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewWhitelist.sol/NewWhitelist.dbg.json
--rw-r--r--   0        0        0    31173 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewWhitelist.sol/NewWhitelist.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/BokkyPooBahsDateTimeLibrary.sol/BokkyPooBahsDateTimeLibrary.dbg.json
--rw-r--r--   0        0        0      701 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/BokkyPooBahsDateTimeLibrary.sol/BokkyPooBahsDateTimeLibrary.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/Spawn.sol/Spawn.dbg.json
--rw-r--r--   0        0        0     1713 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/Spawn.sol/Spawn.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Address.sol/Address.dbg.json
--rw-r--r--   0        0        0      664 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Address.sol/Address.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Context.sol/Context.dbg.json
--rw-r--r--   0        0        0      250 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Context.sol/Context.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Create2.sol/Create2.dbg.json
--rw-r--r--   0        0        0      664 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Create2.sol/Create2.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/IERC20.sol/IERC20.dbg.json
--rw-r--r--   0        0        0     4014 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/IERC20.sol/IERC20.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Ownable.sol/Ownable.dbg.json
--rw-r--r--   0        0        0     1345 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Ownable.sol/Ownable.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/ReentrancyGuard.sol/ReentrancyGuard.dbg.json
--rw-r--r--   0        0        0      266 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/ReentrancyGuard.sol/ReentrancyGuard.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/SafeERC20.sol/SafeERC20.dbg.json
--rw-r--r--   0        0        0      668 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/SafeERC20.sol/SafeERC20.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/SafeMath.sol/SafeMath.dbg.json
--rw-r--r--   0        0        0      666 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/SafeMath.sol/SafeMath.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/SignedSafeMath.sol/SignedSafeMath.dbg.json
--rw-r--r--   0        0        0      678 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/SignedSafeMath.sol/SignedSafeMath.json
--rw-r--r--   0        0        0      117 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Strings.sol/Strings.dbg.json
--rw-r--r--   0        0        0      664 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Strings.sol/Strings.json
--rw-r--r--   0        0        0      120 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ERC20Upgradeable.sol/ERC20Upgradeable.dbg.json
--rw-r--r--   0        0        0    16052 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ERC20Upgradeable.sol/ERC20Upgradeable.json
--rw-r--r--   0        0        0      123 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/GSN/ContextUpgradeable.sol/ContextUpgradeable.dbg.json
--rw-r--r--   0        0        0      291 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/GSN/ContextUpgradeable.sol/ContextUpgradeable.json
--rw-r--r--   0        0        0      120 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/IERC20Upgradeable.sol/IERC20Upgradeable.dbg.json
--rw-r--r--   0        0        0     4051 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/IERC20Upgradeable.sol/IERC20Upgradeable.json
--rw-r--r--   0        0        0      120 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Initializable.sol/Initializable.dbg.json
--rw-r--r--   0        0        0      587 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Initializable.sol/Initializable.json
--rw-r--r--   0        0        0      120 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnableUpgradeSafe.sol/OwnableUpgradeSafe.dbg.json
--rw-r--r--   0        0        0     4294 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnableUpgradeSafe.sol/OwnableUpgradeSafe.json
--rw-r--r--   0        0        0      120 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnedUpgradeabilityProxy.sol/OwnedUpgradeabilityProxy.dbg.json
--rw-r--r--   0        0        0     7531 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnedUpgradeabilityProxy.sol/OwnedUpgradeabilityProxy.json
--rw-r--r--   0        0        0      120 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Proxy.sol/Proxy.dbg.json
--rw-r--r--   0        0        0      595 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Proxy.sol/Proxy.json
--rw-r--r--   0        0        0      120 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ReentrancyGuardUpgradeSafe.sol/ReentrancyGuardUpgradeSafe.dbg.json
--rw-r--r--   0        0        0      613 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ReentrancyGuardUpgradeSafe.sol/ReentrancyGuardUpgradeSafe.json
--rw-r--r--   0        0        0      120 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/UpgradeabilityProxy.sol/UpgradeabilityProxy.dbg.json
--rw-r--r--   0        0        0     2001 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/UpgradeabilityProxy.sol/UpgradeabilityProxy.json
--rw-r--r--   0        0        0      123 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/cryptography/ECDSAUpgradeable.sol/ECDSAUpgradeable.dbg.json
--rw-r--r--   0        0        0      546 2023-06-04 11:48:29.264209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/cryptography/ECDSAUpgradeable.sol/ECDSAUpgradeable.json
--rw-r--r--   0        0        0      123 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/EIP712Upgradeable.sol/EIP712Upgradeable.dbg.json
--rw-r--r--   0        0        0      298 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/EIP712Upgradeable.sol/EIP712Upgradeable.json
--rw-r--r--   0        0        0      123 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/ERC20PermitUpgradeable.sol/ERC20PermitUpgradeable.dbg.json
--rw-r--r--   0        0        0     7379 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/ERC20PermitUpgradeable.sol/ERC20PermitUpgradeable.json
--rw-r--r--   0        0        0      123 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.dbg.json
--rw-r--r--   0        0        0     1870 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.json
--rw-r--r--   0        0        0      123 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/math/SafeMathUpgradeable.sol/SafeMathUpgradeable.dbg.json
--rw-r--r--   0        0        0      544 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/math/SafeMathUpgradeable.sol/SafeMathUpgradeable.json
--rw-r--r--   0        0        0      123 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/utils/CountersUpgradeable.sol/CountersUpgradeable.dbg.json
--rw-r--r--   0        0        0      545 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/utils/CountersUpgradeable.sol/CountersUpgradeable.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/ChainlinkPricer.sol/ChainLinkPricer.dbg.json
--rw-r--r--   0        0        0    12510 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/ChainlinkPricer.sol/ChainLinkPricer.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/CompoundPricer.sol/CompoundPricer.dbg.json
--rw-r--r--   0        0        0    10253 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/CompoundPricer.sol/CompoundPricer.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/WstethPricer.sol/WstethPricer.dbg.json
--rw-r--r--   0        0        0     9115 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/WstethPricer.sol/WstethPricer.json
--rw-r--r--   0        0        0      114 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/YearnPricer.sol/YearnPricer.dbg.json
--rw-r--r--   0        0        0    10339 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/YearnPricer.sol/YearnPricer.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/tokens/ERC20.sol/ERC20.dbg.json
--rw-r--r--   0        0        0     6254 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/tokens/ERC20.sol/ERC20.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/tokens/MintableERC20.sol/MintableERC20.dbg.json
--rw-r--r--   0        0        0    20725 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/tokens/MintableERC20.sol/MintableERC20.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/tokens/WETH.sol/WETH.dbg.json
--rw-r--r--   0        0        0    14042 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/tokens/WETH.sol/WETH.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholes.dbg.json
--rw-r--r--   0        0        0      698 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholes.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholesTest.dbg.json
--rw-r--r--   0        0        0    26324 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholesTest.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/BlackScholesTest.sol/NormalDist.dbg.json
--rw-r--r--   0        0        0      696 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/BlackScholesTest.sol/NormalDist.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/LiquidityPoolAdjustCollateralTest.sol/LiquidityPoolAdjustCollateralTest.dbg.json
--rw-r--r--   0        0        0    14566 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/LiquidityPoolAdjustCollateralTest.sol/LiquidityPoolAdjustCollateralTest.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/OracleMock.sol/OracleMock.dbg.json
--rw-r--r--   0        0        0     7244 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/OracleMock.sol/OracleMock.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/PerpHedgingTest.sol/PerpHedgingTest.dbg.json
--rw-r--r--   0        0        0     8117 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/PerpHedgingTest.sol/PerpHedgingTest.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/RealTokenMock.sol/RealTokenMock.dbg.json
--rw-r--r--   0        0        0    39837 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/RealTokenMock.sol/RealTokenMock.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/ReentrancyGuard.sol/ReentrancyGuard.dbg.json
--rw-r--r--   0        0        0      668 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/ReentrancyGuard.sol/ReentrancyGuard.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/UniswapConversionsTest.sol/UniswapConversionsTest.dbg.json
--rw-r--r--   0        0        0    17149 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/UniswapConversionsTest.sol/UniswapConversionsTest.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/UniswapV3HedgingTest.sol/UniswapV3HedgingTest.dbg.json
--rw-r--r--   0        0        0     8046 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/UniswapV3HedgingTest.sol/UniswapV3HedgingTest.json
--rw-r--r--   0        0        0      108 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/Volatility.sol/Volatility.dbg.json
--rw-r--r--   0        0        0     5933 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/utils/Volatility.sol/Volatility.json
--rw-r--r--   0        0        0      111 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/FullMath.sol/FullMath.dbg.json
--rw-r--r--   0        0        0      695 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/FullMath.sol/FullMath.json
--rw-r--r--   0        0        0      111 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/LiquidityAmounts.sol/LiquidityAmounts.dbg.json
--rw-r--r--   0        0        0      711 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/LiquidityAmounts.sol/LiquidityAmounts.json
--rw-r--r--   0        0        0      111 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/PoolAddress.sol/PoolAddress.dbg.json
--rw-r--r--   0        0        0      701 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/PoolAddress.sol/PoolAddress.json
--rw-r--r--   0        0        0      111 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/TickMath.sol/TickMath.dbg.json
--rw-r--r--   0        0        0      845 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/TickMath.sol/TickMath.json
--rw-r--r--   0        0        0      499 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/src/action_types.py
--rw-r--r--   0        0        0      856 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/src/collateral.py
--rw-r--r--   0        0        0     4643 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/src/constants.py
--rw-r--r--   0        0        0     2301 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/src/pnl_calculator.py
--rw-r--r--   0        0        0     1920 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/src/position.py
--rw-r--r--   0        0        0     2432 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/src/rysk_option_market.py
--rw-r--r--   0        0        0     3106 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/src/subgraph.py
--rw-r--r--   0        0        0     1914 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/src/utils.py
--rw-r--r--   0        0        0     2991 2023-06-04 11:48:29.268209 rysk_client-0.1.8/rysk_client/web3_client.py
--rw-r--r--   0        0        0    27227 1970-01-01 00:00:00.000000 rysk_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    27832 2023-06-09 09:37:41.342633 rysk_client-0.1.9/README.md
+-rw-r--r--   0        0        0      603 2023-06-09 09:37:41.346633 rysk_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/__init__.py
+-rw-r--r--   0        0        0     5521 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/cli.py
+-rw-r--r--   0        0        0    22266 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/client.py
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/Accounting.sol/Accounting.dbg.json
+-rw-r--r--   0        0        0    32509 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/Accounting.sol/Accounting.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/AlphaOptionHandler.sol/AlphaOptionHandler.dbg.json
+-rw-r--r--   0        0        0    55200 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/AlphaOptionHandler.sol/AlphaOptionHandler.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/AlphaPortfolioValuesFeed.sol/AlphaPortfolioValuesFeed.dbg.json
+-rw-r--r--   0        0        0    58641 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/AlphaPortfolioValuesFeed.sol/AlphaPortfolioValuesFeed.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/Authority.sol/Authority.dbg.json
+-rw-r--r--   0        0        0    14683 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/Authority.sol/Authority.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/BeyondPricer.sol/BeyondPricer.dbg.json
+-rw-r--r--   0        0        0    69533 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/BeyondPricer.sol/BeyondPricer.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/LiquidityPool.sol/LiquidityPool.dbg.json
+-rw-r--r--   0        0        0   134569 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/LiquidityPool.sol/LiquidityPool.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.346633 rysk_client-0.1.9/rysk_client/contracts/Manager.sol/Manager.dbg.json
+-rw-r--r--   0        0        0    43720 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/Manager.sol/Manager.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/OptionCatalogue.sol/OptionCatalogue.dbg.json
+-rw-r--r--   0        0        0    30256 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/OptionCatalogue.sol/OptionCatalogue.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/OptionExchange.sol/OptionExchange.dbg.json
+-rw-r--r--   0        0        0   129629 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/OptionExchange.sol/OptionExchange.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/OptionRegistry.sol/OptionRegistry.dbg.json
+-rw-r--r--   0        0        0   105395 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/OptionRegistry.sol/OptionRegistry.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/PriceFeed.sol/PriceFeed.dbg.json
+-rw-r--r--   0        0        0    16525 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/PriceFeed.sol/PriceFeed.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/Protocol.sol/Protocol.dbg.json
+-rw-r--r--   0        0        0     9497 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/Protocol.sol/Protocol.json
+-rw-r--r--   0        0        0      105 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/VolatilityFeed.sol/VolatilityFeed.dbg.json
+-rw-r--r--   0        0        0    50343 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/VolatilityFeed.sol/VolatilityFeed.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/gelato/OpynPricerResolver.sol/OpynPricerResolver.dbg.json
+-rw-r--r--   0        0        0     9140 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/gelato/OpynPricerResolver.sol/OpynPricerResolver.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/gelato/VaultCollateralMulticall.sol/VaultCollateralMulticall.dbg.json
+-rw-r--r--   0        0        0     8662 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/gelato/VaultCollateralMulticall.sol/VaultCollateralMulticall.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/hedging/GmxHedgingReactor.sol/GmxHedgingReactor.dbg.json
+-rw-r--r--   0        0        0    89973 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/hedging/GmxHedgingReactor.sol/GmxHedgingReactor.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/hedging/PerpHedgingReactor.sol/PerpHedgingReactor.dbg.json
+-rw-r--r--   0        0        0    59661 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/hedging/PerpHedgingReactor.sol/PerpHedgingReactor.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.350633 rysk_client-0.1.9/rysk_client/contracts/hedging/UniswapV3HedgingReactor.sol/UniswapV3HedgingReactor.dbg.json
+-rw-r--r--   0        0        0    34523 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/hedging/UniswapV3HedgingReactor.sol/UniswapV3HedgingReactor.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/hedging/UniswapV3RangeOrderReactor.sol/UniswapV3RangeOrderReactor.dbg.json
+-rw-r--r--   0        0        0    91201 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/hedging/UniswapV3RangeOrderReactor.sol/UniswapV3RangeOrderReactor.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/AddressBookInterface.sol/AddressBookInterface.dbg.json
+-rw-r--r--   0        0        0     5293 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/AddressBookInterface.sol/AddressBookInterface.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/AggregatorInterface.sol/AggregatorInterface.dbg.json
+-rw-r--r--   0        0        0     5198 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/AggregatorInterface.sol/AggregatorInterface.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/AggregatorV3Interface.sol/AggregatorV3Interface.dbg.json
+-rw-r--r--   0        0        0     2596 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/AggregatorV3Interface.sol/AggregatorV3Interface.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/GammaTypes.dbg.json
+-rw-r--r--   0        0        0      699 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/GammaTypes.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/IController.dbg.json
+-rw-r--r--   0        0        0     7300 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/IController.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/IOtoken.dbg.json
+-rw-r--r--   0        0        0     1774 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/IOtoken.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/IOtokenFactory.dbg.json
+-rw-r--r--   0        0        0     4447 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/IOtokenFactory.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAccounting.sol/IAccounting.dbg.json
+-rw-r--r--   0        0        0     5466 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAccounting.sol/IAccounting.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAddressBook.sol/IAddressBook.dbg.json
+-rw-r--r--   0        0        0      500 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAddressBook.sol/IAddressBook.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAlphaOptionHandler.sol/IAlphaOptionHandler.dbg.json
+-rw-r--r--   0        0        0     5572 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAlphaOptionHandler.sol/IAlphaOptionHandler.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAlphaPortfolioValuesFeed.sol/IAlphaPortfolioValuesFeed.dbg.json
+-rw-r--r--   0        0        0     6033 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAlphaPortfolioValuesFeed.sol/IAlphaPortfolioValuesFeed.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAuthority.sol/IAuthority.dbg.json
+-rw-r--r--   0        0        0     3351 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IAuthority.sol/IAuthority.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IChainlinkPricer.sol/IChainlinkPricer.dbg.json
+-rw-r--r--   0        0        0      657 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IChainlinkPricer.sol/IChainlinkPricer.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IGmxVault.sol/IGmxVault.dbg.json
+-rw-r--r--   0        0        0    35992 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IGmxVault.sol/IGmxVault.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IGmxVaultPriceFeed.sol/IVaultPriceFeed.dbg.json
+-rw-r--r--   0        0        0     6762 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IGmxVaultPriceFeed.sol/IVaultPriceFeed.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IHedgingReactor.sol/IHedgingReactor.dbg.json
+-rw-r--r--   0        0        0     1789 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IHedgingReactor.sol/IHedgingReactor.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/ILiquidityPool.sol/ILiquidityPool.dbg.json
+-rw-r--r--   0        0        0    21076 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/ILiquidityPool.sol/ILiquidityPool.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.354633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IMarginCalculator.sol/IMarginCalculator.dbg.json
+-rw-r--r--   0        0        0     1610 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IMarginCalculator.sol/IMarginCalculator.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IOptionRegistry.sol/IOptionRegistry.dbg.json
+-rw-r--r--   0        0        0     8964 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IOptionRegistry.sol/IOptionRegistry.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IOracle.sol/IOracle.dbg.json
+-rw-r--r--   0        0        0     1714 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IOracle.sol/IOracle.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IPortfolioValuesFeed.sol/IPortfolioValuesFeed.dbg.json
+-rw-r--r--   0        0        0     3777 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IPortfolioValuesFeed.sol/IPortfolioValuesFeed.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IPositionRouter.sol/IPositionRouter.dbg.json
+-rw-r--r--   0        0        0     7286 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IPositionRouter.sol/IPositionRouter.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IPriceFeedTimelock.sol/IPriceFeedTimelock.dbg.json
+-rw-r--r--   0        0        0     2430 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IPriceFeedTimelock.sol/IPriceFeedTimelock.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IReader.sol/IReader.dbg.json
+-rw-r--r--   0        0        0     1099 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IReader.sol/IReader.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IRouter.sol/IRouter.dbg.json
+-rw-r--r--   0        0        0     4125 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IRouter.sol/IRouter.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IWhitelist.sol/IWhitelist.dbg.json
+-rw-r--r--   0        0        0     3225 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/IWhitelist.sol/IWhitelist.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/I_ERC20.sol/I_ERC20.dbg.json
+-rw-r--r--   0        0        0     4001 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/I_ERC20.sol/I_ERC20.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/OtokenInterface.sol/OtokenInterface.dbg.json
+-rw-r--r--   0        0        0     4570 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/OtokenInterface.sol/OtokenInterface.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/WETH.sol/WETH.dbg.json
+-rw-r--r--   0        0        0     3229 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/interfaces/WETH.sol/WETH.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/lens/DHVLensMK1.sol/DHVLensMK1.dbg.json
+-rw-r--r--   0        0        0    40159 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/lens/DHVLensMK1.sol/DHVLensMK1.json
+-rw-r--r--   0        0        0      956 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/lens/UserPositionLensMK1.sol/UserPositionLensMK1.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/AccessControl.sol/AccessControl.dbg.json
+-rw-r--r--   0        0        0     1163 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/AccessControl.sol/AccessControl.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/BlackScholes.sol/BlackScholes.dbg.json
+-rw-r--r--   0        0        0    37568 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/BlackScholes.sol/BlackScholes.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/CombinedActions.sol/CombinedActions.dbg.json
+-rw-r--r--   0        0        0      704 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/CombinedActions.sol/CombinedActions.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/CustomErrors.sol/CustomErrors.dbg.json
+-rw-r--r--   0        0        0     7217 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/CustomErrors.sol/CustomErrors.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/EnumerableSet.sol/EnumerableSet.dbg.json
+-rw-r--r--   0        0        0      700 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/EnumerableSet.sol/EnumerableSet.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/NormalDist.sol/NormalDist.dbg.json
+-rw-r--r--   0        0        0    18234 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/NormalDist.sol/NormalDist.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/OptionsCompute.sol/OptionsCompute.dbg.json
+-rw-r--r--   0        0        0     9215 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/OptionsCompute.sol/OptionsCompute.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/OpynInteractions.sol/OpynInteractions.dbg.json
+-rw-r--r--   0        0        0    33677 2023-06-09 09:37:41.358633 rysk_client-0.1.9/rysk_client/contracts/libraries/OpynInteractions.sol/OpynInteractions.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/libraries/RyskActions.sol/RyskActions.dbg.json
+-rw-r--r--   0        0        0      696 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/libraries/RyskActions.sol/RyskActions.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/libraries/SABR.sol/SABR.dbg.json
+-rw-r--r--   0        0        0      682 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/libraries/SABR.sol/SABR.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/libraries/SafeTransferLib.sol/SafeTransferLib.dbg.json
+-rw-r--r--   0        0        0      704 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/libraries/SafeTransferLib.sol/SafeTransferLib.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/libraries/Types.sol/Types.dbg.json
+-rw-r--r--   0        0        0      684 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/libraries/Types.sol/Types.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/mocks/ForceSend.sol/ForceSend.dbg.json
+-rw-r--r--   0        0        0     1207 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/mocks/ForceSend.sol/ForceSend.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/mocks/MockChainlinkAggregator.sol/MockChainlinkAggregator.dbg.json
+-rw-r--r--   0        0        0     6246 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/mocks/MockChainlinkAggregator.sol/MockChainlinkAggregator.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/mocks/MockChainlinkSequencerFeed.sol/MockChainlinkSequencerFeed.dbg.json
+-rw-r--r--   0        0        0     2861 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/mocks/MockChainlinkSequencerFeed.sol/MockChainlinkSequencerFeed.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/mocks/MockPortfolioValuesFeed.sol/MockPortfolioValuesFeed.dbg.json
+-rw-r--r--   0        0        0    23550 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/mocks/MockPortfolioValuesFeed.sol/MockPortfolioValuesFeed.json
+-rw-r--r--   0        0        0     4355 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/otoken.json
+-rw-r--r--   0        0        0      111 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/Migrations.sol/Migrations.dbg.json
+-rw-r--r--   0        0        0     2244 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/Migrations.sol/Migrations.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/AddressBook.sol/AddressBook.dbg.json
+-rw-r--r--   0        0        0    27786 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/AddressBook.sol/AddressBook.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Controller.sol/Controller.dbg.json
+-rw-r--r--   0        0        0   127044 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Controller.sol/Controller.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/MarginCalculator.sol/MarginCalculator.dbg.json
+-rw-r--r--   0        0        0    89218 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/MarginCalculator.sol/MarginCalculator.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/MarginPool.sol/MarginPool.dbg.json
+-rw-r--r--   0        0        0    30610 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/MarginPool.sol/MarginPool.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Oracle.sol/Oracle.dbg.json
+-rw-r--r--   0        0        0    36101 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Oracle.sol/Oracle.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Otoken.sol/Otoken.dbg.json
+-rw-r--r--   0        0        0    60378 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Otoken.sol/Otoken.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/OtokenFactory.sol/OtokenFactory.dbg.json
+-rw-r--r--   0        0        0    24205 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/OtokenFactory.sol/OtokenFactory.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/OtokenSpawner.sol/OtokenSpawner.dbg.json
+-rw-r--r--   0        0        0      565 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/OtokenSpawner.sol/OtokenSpawner.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Whitelist.sol/Whitelist.dbg.json
+-rw-r--r--   0        0        0    24760 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Whitelist.sol/Whitelist.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/external/callees/PermitCallee.sol/PermitCallee.dbg.json
+-rw-r--r--   0        0        0     3477 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/external/callees/PermitCallee.sol/PermitCallee.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/external/canonical-weth/WETH9.sol/WETH9.dbg.json
+-rw-r--r--   0        0        0    14660 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/external/canonical-weth/WETH9.sol/WETH9.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.362633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/external/proxies/PayableProxyController.sol/PayableProxyController.dbg.json
+-rw-r--r--   0        0        0    21982 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/external/proxies/PayableProxyController.sol/PayableProxyController.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/AddressBookInterface.sol/AddressBookInterface.dbg.json
+-rw-r--r--   0        0        0     5307 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/AddressBookInterface.sol/AddressBookInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/AggregatorInterface.sol/AggregatorInterface.dbg.json
+-rw-r--r--   0        0        0     5212 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/AggregatorInterface.sol/AggregatorInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/CTokenInterface.sol/CTokenInterface.dbg.json
+-rw-r--r--   0        0        0      781 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/CTokenInterface.sol/CTokenInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/CalleeInterface.sol/CalleeInterface.dbg.json
+-rw-r--r--   0        0        0      653 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/CalleeInterface.sol/CalleeInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/ERC20Interface.sol/ERC20Interface.dbg.json
+-rw-r--r--   0        0        0     4639 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/ERC20Interface.sol/ERC20Interface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/MarginCalculatorInterface.sol/MarginCalculatorInterface.dbg.json
+-rw-r--r--   0        0        0     4342 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/MarginCalculatorInterface.sol/MarginCalculatorInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/MarginPoolInterface.sol/MarginPoolInterface.dbg.json
+-rw-r--r--   0        0        0     3944 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/MarginPoolInterface.sol/MarginPoolInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/OpynPricerInterface.sol/OpynPricerInterface.dbg.json
+-rw-r--r--   0        0        0     1017 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/OpynPricerInterface.sol/OpynPricerInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/OracleInterface.sol/OracleInterface.dbg.json
+-rw-r--r--   0        0        0     7103 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/OracleInterface.sol/OracleInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/OtokenInterface.sol/OtokenInterface.dbg.json
+-rw-r--r--   0        0        0     4584 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/OtokenInterface.sol/OtokenInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/WETH9Interface.sol/WETH9Interface.dbg.json
+-rw-r--r--   0        0        0     2475 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/WETH9Interface.sol/WETH9Interface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/WSTETHInterface.sol/WSTETHInterface.dbg.json
+-rw-r--r--   0        0        0     1266 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/WSTETHInterface.sol/WSTETHInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/WhitelistInterface.sol/WhitelistInterface.dbg.json
+-rw-r--r--   0        0        0     7545 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/WhitelistInterface.sol/WhitelistInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/YearnVaultInterface.sol/YearnVaultInterface.dbg.json
+-rw-r--r--   0        0        0     1789 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/YearnVaultInterface.sol/YearnVaultInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/ZeroXExchangeInterface.sol/ZeroXExchangeInterface.dbg.json
+-rw-r--r--   0        0        0     3503 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/ZeroXExchangeInterface.sol/ZeroXExchangeInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/Actions.sol/Actions.dbg.json
+-rw-r--r--   0        0        0      657 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/Actions.sol/Actions.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/FixedPointInt256.sol/FixedPointInt256.dbg.json
+-rw-r--r--   0        0        0      675 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/FixedPointInt256.sol/FixedPointInt256.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/MarginVault.sol/MarginVault.dbg.json
+-rw-r--r--   0        0        0    11131 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/MarginVault.sol/MarginVault.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/SignedConverter.sol/SignedConverter.dbg.json
+-rw-r--r--   0        0        0      673 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/SignedConverter.sol/SignedConverter.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewCalculator.sol/NewMarginCalculator.dbg.json
+-rw-r--r--   0        0        0    94183 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewCalculator.sol/NewMarginCalculator.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewController.sol/NewController.dbg.json
+-rw-r--r--   0        0        0   129863 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewController.sol/NewController.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewMarginCalculatorInterface.sol/MarginCalculatorInterface.dbg.json
+-rw-r--r--   0        0        0     4096 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewMarginCalculatorInterface.sol/MarginCalculatorInterface.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewWhitelist.sol/NewWhitelist.dbg.json
+-rw-r--r--   0        0        0    31173 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewWhitelist.sol/NewWhitelist.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/BokkyPooBahsDateTimeLibrary.sol/BokkyPooBahsDateTimeLibrary.dbg.json
+-rw-r--r--   0        0        0      701 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/BokkyPooBahsDateTimeLibrary.sol/BokkyPooBahsDateTimeLibrary.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/Spawn.sol/Spawn.dbg.json
+-rw-r--r--   0        0        0     1713 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/Spawn.sol/Spawn.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Address.sol/Address.dbg.json
+-rw-r--r--   0        0        0      664 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Address.sol/Address.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Context.sol/Context.dbg.json
+-rw-r--r--   0        0        0      250 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Context.sol/Context.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Create2.sol/Create2.dbg.json
+-rw-r--r--   0        0        0      664 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Create2.sol/Create2.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/IERC20.sol/IERC20.dbg.json
+-rw-r--r--   0        0        0     4014 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/IERC20.sol/IERC20.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Ownable.sol/Ownable.dbg.json
+-rw-r--r--   0        0        0     1345 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Ownable.sol/Ownable.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/ReentrancyGuard.sol/ReentrancyGuard.dbg.json
+-rw-r--r--   0        0        0      266 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/ReentrancyGuard.sol/ReentrancyGuard.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/SafeERC20.sol/SafeERC20.dbg.json
+-rw-r--r--   0        0        0      668 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/SafeERC20.sol/SafeERC20.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.366633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/SafeMath.sol/SafeMath.dbg.json
+-rw-r--r--   0        0        0      666 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/SafeMath.sol/SafeMath.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/SignedSafeMath.sol/SignedSafeMath.dbg.json
+-rw-r--r--   0        0        0      678 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/SignedSafeMath.sol/SignedSafeMath.json
+-rw-r--r--   0        0        0      117 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Strings.sol/Strings.dbg.json
+-rw-r--r--   0        0        0      664 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Strings.sol/Strings.json
+-rw-r--r--   0        0        0      120 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ERC20Upgradeable.sol/ERC20Upgradeable.dbg.json
+-rw-r--r--   0        0        0    16052 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ERC20Upgradeable.sol/ERC20Upgradeable.json
+-rw-r--r--   0        0        0      123 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/GSN/ContextUpgradeable.sol/ContextUpgradeable.dbg.json
+-rw-r--r--   0        0        0      291 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/GSN/ContextUpgradeable.sol/ContextUpgradeable.json
+-rw-r--r--   0        0        0      120 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/IERC20Upgradeable.sol/IERC20Upgradeable.dbg.json
+-rw-r--r--   0        0        0     4051 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/IERC20Upgradeable.sol/IERC20Upgradeable.json
+-rw-r--r--   0        0        0      120 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Initializable.sol/Initializable.dbg.json
+-rw-r--r--   0        0        0      587 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Initializable.sol/Initializable.json
+-rw-r--r--   0        0        0      120 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnableUpgradeSafe.sol/OwnableUpgradeSafe.dbg.json
+-rw-r--r--   0        0        0     4294 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnableUpgradeSafe.sol/OwnableUpgradeSafe.json
+-rw-r--r--   0        0        0      120 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnedUpgradeabilityProxy.sol/OwnedUpgradeabilityProxy.dbg.json
+-rw-r--r--   0        0        0     7531 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnedUpgradeabilityProxy.sol/OwnedUpgradeabilityProxy.json
+-rw-r--r--   0        0        0      120 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Proxy.sol/Proxy.dbg.json
+-rw-r--r--   0        0        0      595 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Proxy.sol/Proxy.json
+-rw-r--r--   0        0        0      120 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ReentrancyGuardUpgradeSafe.sol/ReentrancyGuardUpgradeSafe.dbg.json
+-rw-r--r--   0        0        0      613 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ReentrancyGuardUpgradeSafe.sol/ReentrancyGuardUpgradeSafe.json
+-rw-r--r--   0        0        0      120 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/UpgradeabilityProxy.sol/UpgradeabilityProxy.dbg.json
+-rw-r--r--   0        0        0     2001 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/UpgradeabilityProxy.sol/UpgradeabilityProxy.json
+-rw-r--r--   0        0        0      123 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/cryptography/ECDSAUpgradeable.sol/ECDSAUpgradeable.dbg.json
+-rw-r--r--   0        0        0      546 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/cryptography/ECDSAUpgradeable.sol/ECDSAUpgradeable.json
+-rw-r--r--   0        0        0      123 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/EIP712Upgradeable.sol/EIP712Upgradeable.dbg.json
+-rw-r--r--   0        0        0      298 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/EIP712Upgradeable.sol/EIP712Upgradeable.json
+-rw-r--r--   0        0        0      123 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/ERC20PermitUpgradeable.sol/ERC20PermitUpgradeable.dbg.json
+-rw-r--r--   0        0        0     7379 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/ERC20PermitUpgradeable.sol/ERC20PermitUpgradeable.json
+-rw-r--r--   0        0        0      123 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.dbg.json
+-rw-r--r--   0        0        0     1870 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.json
+-rw-r--r--   0        0        0      123 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/math/SafeMathUpgradeable.sol/SafeMathUpgradeable.dbg.json
+-rw-r--r--   0        0        0      544 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/math/SafeMathUpgradeable.sol/SafeMathUpgradeable.json
+-rw-r--r--   0        0        0      123 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/utils/CountersUpgradeable.sol/CountersUpgradeable.dbg.json
+-rw-r--r--   0        0        0      545 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/utils/CountersUpgradeable.sol/CountersUpgradeable.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/ChainlinkPricer.sol/ChainLinkPricer.dbg.json
+-rw-r--r--   0        0        0    12510 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/ChainlinkPricer.sol/ChainLinkPricer.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/CompoundPricer.sol/CompoundPricer.dbg.json
+-rw-r--r--   0        0        0    10253 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/CompoundPricer.sol/CompoundPricer.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/WstethPricer.sol/WstethPricer.dbg.json
+-rw-r--r--   0        0        0     9115 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/WstethPricer.sol/WstethPricer.json
+-rw-r--r--   0        0        0      114 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/YearnPricer.sol/YearnPricer.dbg.json
+-rw-r--r--   0        0        0    10339 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/YearnPricer.sol/YearnPricer.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/tokens/ERC20.sol/ERC20.dbg.json
+-rw-r--r--   0        0        0     6254 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/tokens/ERC20.sol/ERC20.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/tokens/MintableERC20.sol/MintableERC20.dbg.json
+-rw-r--r--   0        0        0    20725 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/tokens/MintableERC20.sol/MintableERC20.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/tokens/WETH.sol/WETH.dbg.json
+-rw-r--r--   0        0        0    14042 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/tokens/WETH.sol/WETH.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholes.dbg.json
+-rw-r--r--   0        0        0      698 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholes.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholesTest.dbg.json
+-rw-r--r--   0        0        0    26324 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholesTest.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/BlackScholesTest.sol/NormalDist.dbg.json
+-rw-r--r--   0        0        0      696 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/BlackScholesTest.sol/NormalDist.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/LiquidityPoolAdjustCollateralTest.sol/LiquidityPoolAdjustCollateralTest.dbg.json
+-rw-r--r--   0        0        0    14566 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/LiquidityPoolAdjustCollateralTest.sol/LiquidityPoolAdjustCollateralTest.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/OracleMock.sol/OracleMock.dbg.json
+-rw-r--r--   0        0        0     7244 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/OracleMock.sol/OracleMock.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/PerpHedgingTest.sol/PerpHedgingTest.dbg.json
+-rw-r--r--   0        0        0     8117 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/PerpHedgingTest.sol/PerpHedgingTest.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.370633 rysk_client-0.1.9/rysk_client/contracts/utils/RealTokenMock.sol/RealTokenMock.dbg.json
+-rw-r--r--   0        0        0    39837 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/utils/RealTokenMock.sol/RealTokenMock.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/utils/ReentrancyGuard.sol/ReentrancyGuard.dbg.json
+-rw-r--r--   0        0        0      668 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/utils/ReentrancyGuard.sol/ReentrancyGuard.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/utils/UniswapConversionsTest.sol/UniswapConversionsTest.dbg.json
+-rw-r--r--   0        0        0    17149 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/utils/UniswapConversionsTest.sol/UniswapConversionsTest.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/utils/UniswapV3HedgingTest.sol/UniswapV3HedgingTest.dbg.json
+-rw-r--r--   0        0        0     8046 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/utils/UniswapV3HedgingTest.sol/UniswapV3HedgingTest.json
+-rw-r--r--   0        0        0      108 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/utils/Volatility.sol/Volatility.dbg.json
+-rw-r--r--   0        0        0     5933 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/utils/Volatility.sol/Volatility.json
+-rw-r--r--   0        0        0      111 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/FullMath.sol/FullMath.dbg.json
+-rw-r--r--   0        0        0      695 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/FullMath.sol/FullMath.json
+-rw-r--r--   0        0        0      111 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/LiquidityAmounts.sol/LiquidityAmounts.dbg.json
+-rw-r--r--   0        0        0      711 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/LiquidityAmounts.sol/LiquidityAmounts.json
+-rw-r--r--   0        0        0      111 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/PoolAddress.sol/PoolAddress.dbg.json
+-rw-r--r--   0        0        0      701 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/PoolAddress.sol/PoolAddress.json
+-rw-r--r--   0        0        0      111 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/TickMath.sol/TickMath.dbg.json
+-rw-r--r--   0        0        0      845 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/TickMath.sol/TickMath.json
+-rw-r--r--   0        0        0      499 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/src/action_types.py
+-rw-r--r--   0        0        0      860 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/src/collateral.py
+-rw-r--r--   0        0        0     5573 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/src/constants.py
+-rw-r--r--   0        0        0      212 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/src/crypto.py
+-rw-r--r--   0        0        0     4538 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/src/pnl_calculator.py
+-rw-r--r--   0        0        0     2096 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/src/position.py
+-rw-r--r--   0        0        0     7530 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/src/rysk_option_market.py
+-rw-r--r--   0        0        0     3106 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/src/subgraph.py
+-rw-r--r--   0        0        0     1914 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/src/utils.py
+-rw-r--r--   0        0        0     9876 2023-06-09 09:37:41.374633 rysk_client-0.1.9/rysk_client/web3_client.py
+-rw-r--r--   0        0        0    28377 1970-01-01 00:00:00.000000 rysk_client-0.1.9/PKG-INFO
```

### Comparing `rysk_client-0.1.8/README.md` & `rysk_client-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,83 +1,104 @@
 # Rysk Client
 
 ## Installation
 
-### Dev
+The application is availale on pypi and can be installed as so;
 
-dependencies are managed with poetry. 
+    ```bash
+    pip install rysk-client
+    ```
+
+### Dev & Contributing
+
+Dependencies are managed with poetry.
 
 For dev build.
 
 
 ```python
-!pip install rysk-client
+!pip install -U .
 ```
 
-    Requirement already satisfied: rysk-client in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (0.1.3)
-    Requirement already satisfied: web3<6.0.0,>=5.4.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client) (5.25.0)
-    Requirement already satisfied: ccxt<4.0.0,>=3.1.15 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client) (3.1.17)
-    Requirement already satisfied: requests>=2.18.4 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (2.28.1)
-    Requirement already satisfied: cryptography>=2.6.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (39.0.1)
-    Requirement already satisfied: setuptools>=60.9.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (67.8.0)
-    Requirement already satisfied: aiodns>=1.1.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (3.0.0)
-    Requirement already satisfied: certifi>=2018.1.18 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (2022.6.15)
-    Requirement already satisfied: aiohttp>=3.8 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (3.8.4)
-    Requirement already satisfied: yarl>=1.7.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (1.7.2)
-    Requirement already satisfied: protobuf<4,>=3.10.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (3.20.3)
-    Requirement already satisfied: eth-typing<3.0.0,>=2.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (2.3.0)
-    Requirement already satisfied: hexbytes<1.0.0,>=0.1.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (0.3.0)
-    Requirement already satisfied: eth-utils<2.0.0,>=1.9.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (1.9.5)
-    Requirement already satisfied: websockets<10,>=9.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (9.1)
-    Requirement already satisfied: lru-dict<2.0.0,>=1.1.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (1.1.8)
-    Requirement already satisfied: eth-account<0.6.0,>=0.5.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (0.5.6)
-    Requirement already satisfied: eth-hash[pycryptodome]<1.0.0,>=0.2.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (0.5.0)
-    Requirement already satisfied: ipfshttpclient==0.8.0a2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (0.8.0a2)
-    Requirement already satisfied: jsonschema<4.0.0,>=3.2.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (3.2.0)
-    Requirement already satisfied: eth-abi<3.0.0,>=2.0.0b6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (2.2.0)
-    Requirement already satisfied: multiaddr>=0.0.7 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ipfshttpclient==0.8.0a2->web3<6.0.0,>=5.4.0->rysk-client) (0.0.9)
-    Requirement already satisfied: pycares>=4.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiodns>=1.1.1->ccxt<4.0.0,>=3.1.15->rysk-client) (4.2.2)
-    Requirement already satisfied: multidict<7.0,>=4.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (6.0.2)
-    Requirement already satisfied: async-timeout<5.0,>=4.0.0a3 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (4.0.2)
-    Requirement already satisfied: attrs>=17.3.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (22.1.0)
-    Requirement already satisfied: charset-normalizer<4.0,>=2.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (2.1.1)
-    Requirement already satisfied: frozenlist>=1.1.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (1.3.1)
-    Requirement already satisfied: aiosignal>=1.1.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (1.2.0)
-    Requirement already satisfied: cffi>=1.12 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cryptography>=2.6.1->ccxt<4.0.0,>=3.1.15->rysk-client) (1.15.1)
-    Requirement already satisfied: parsimonious<0.9.0,>=0.8.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-abi<3.0.0,>=2.0.0b6->web3<6.0.0,>=5.4.0->rysk-client) (0.8.1)
-    Requirement already satisfied: rlp<3,>=1.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (2.0.1)
-    Requirement already satisfied: eth-rlp<2,>=0.1.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (0.2.1)
-    Requirement already satisfied: bitarray<1.3.0,>=1.2.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (1.2.2)
-    Requirement already satisfied: eth-keyfile<0.6.0,>=0.5.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (0.5.1)
-    Requirement already satisfied: eth-keys!=0.3.2,<0.4.0,>=0.2.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (0.3.4)
-    Requirement already satisfied: pycryptodome<4,>=3.6.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-hash[pycryptodome]<1.0.0,>=0.2.0->web3<6.0.0,>=5.4.0->rysk-client) (3.15.0)
-    Requirement already satisfied: cytoolz<1.0.0,>=0.10.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-utils<2.0.0,>=1.9.5->web3<6.0.0,>=5.4.0->rysk-client) (0.12.0)
-    Requirement already satisfied: pyrsistent>=0.14.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from jsonschema<4.0.0,>=3.2.0->web3<6.0.0,>=5.4.0->rysk-client) (0.18.1)
-    Requirement already satisfied: six>=1.11.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from jsonschema<4.0.0,>=3.2.0->web3<6.0.0,>=5.4.0->rysk-client) (1.16.0)
-    Requirement already satisfied: idna<4,>=2.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from requests>=2.18.4->ccxt<4.0.0,>=3.1.15->rysk-client) (3.3)
-    Requirement already satisfied: urllib3<1.27,>=1.21.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from requests>=2.18.4->ccxt<4.0.0,>=3.1.15->rysk-client) (1.26.12)
-    Requirement already satisfied: pycparser in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cffi>=1.12->cryptography>=2.6.1->ccxt<4.0.0,>=3.1.15->rysk-client) (2.21)
-    Requirement already satisfied: toolz>=0.8.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cytoolz<1.0.0,>=0.10.1->eth-utils<2.0.0,>=1.9.5->web3<6.0.0,>=5.4.0->rysk-client) (0.11.2)
-    Requirement already satisfied: netaddr in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from multiaddr>=0.0.7->ipfshttpclient==0.8.0a2->web3<6.0.0,>=5.4.0->rysk-client) (0.8.0)
-    Requirement already satisfied: base58 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from multiaddr>=0.0.7->ipfshttpclient==0.8.0a2->web3<6.0.0,>=5.4.0->rysk-client) (2.1.1)
-    Requirement already satisfied: varint in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from multiaddr>=0.0.7->ipfshttpclient==0.8.0a2->web3<6.0.0,>=5.4.0->rysk-client) (1.0.2)
+    Processing /home/tom/Desktop/Fun/rysk_explorations
+      Installing build dependencies ... [?25ldone
+    [?25h  Getting requirements to build wheel ... [?25ldone
+    [?25h  Preparing metadata (pyproject.toml) ... [?25ldone
+    [?25hRequirement already satisfied: web3==6.4.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client==0.1.8) (6.4.0)
+    Requirement already satisfied: ccxt<4.0.0,>=3.1.15 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client==0.1.8) (3.1.17)
+    Requirement already satisfied: rich-click<2.0.0,>=1.6.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client==0.1.8) (1.6.1)
+    Requirement already satisfied: jsonschema>=4.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (4.17.3)
+    Requirement already satisfied: requests>=2.16.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (2.28.1)
+    Requirement already satisfied: eth-abi>=4.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (4.0.0)
+    Requirement already satisfied: eth-account>=0.8.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (0.9.0)
+    Requirement already satisfied: aiohttp>=3.7.4.post0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (3.8.4)
+    Requirement already satisfied: eth-hash[pycryptodome]>=0.5.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (0.5.2)
+    Requirement already satisfied: hexbytes>=0.1.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (0.3.0)
+    Requirement already satisfied: lru-dict>=1.1.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (1.1.8)
+    Requirement already satisfied: eth-typing>=3.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (3.4.0)
+    Requirement already satisfied: eth-utils>=2.1.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (2.1.1)
+    Requirement already satisfied: protobuf>=4.21.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (4.23.2)
+    Requirement already satisfied: websockets>=10.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (11.0.3)
+    Requirement already satisfied: cryptography>=2.6.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (39.0.1)
+    Requirement already satisfied: aiodns>=1.1.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (3.0.0)
+    Requirement already satisfied: certifi>=2018.1.18 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (2022.6.15)
+    Requirement already satisfied: yarl>=1.7.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (1.7.2)
+    Requirement already satisfied: setuptools>=60.9.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (67.8.0)
+    Requirement already satisfied: rich>=10.7.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (13.3.1)
+    Requirement already satisfied: click>=7 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (8.0.2)
+    Requirement already satisfied: pycares>=4.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiodns>=1.1.1->ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (4.2.2)
+    Requirement already satisfied: charset-normalizer<4.0,>=2.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (2.1.1)
+    Requirement already satisfied: frozenlist>=1.1.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (1.3.1)
+    Requirement already satisfied: async-timeout<5.0,>=4.0.0a3 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (4.0.2)
+    Requirement already satisfied: aiosignal>=1.1.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (1.2.0)
+    Requirement already satisfied: multidict<7.0,>=4.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (6.0.2)
+    Requirement already satisfied: attrs>=17.3.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (22.1.0)
+    Requirement already satisfied: cffi>=1.12 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cryptography>=2.6.1->ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (1.15.1)
+    Requirement already satisfied: parsimonious<0.10.0,>=0.9.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-abi>=4.0.0->web3==6.4.0->rysk-client==0.1.8) (0.9.0)
+    Requirement already satisfied: eth-rlp>=0.3.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (0.3.0)
+    Requirement already satisfied: rlp>=1.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (3.0.0)
+    Requirement already satisfied: eth-keys>=0.4.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (0.4.0)
+    Requirement already satisfied: eth-keyfile>=0.6.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (0.6.1)
+    Requirement already satisfied: bitarray>=2.4.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (2.7.4)
+    Requirement already satisfied: pycryptodome<4,>=3.6.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-hash[pycryptodome]>=0.5.1->web3==6.4.0->rysk-client==0.1.8) (3.15.0)
+    Requirement already satisfied: cytoolz>=0.10.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-utils>=2.1.0->web3==6.4.0->rysk-client==0.1.8) (0.12.0)
+    Requirement already satisfied: pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from jsonschema>=4.0.0->web3==6.4.0->rysk-client==0.1.8) (0.18.1)
+    Requirement already satisfied: urllib3<1.27,>=1.21.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from requests>=2.16.0->web3==6.4.0->rysk-client==0.1.8) (1.26.12)
+    Requirement already satisfied: idna<4,>=2.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from requests>=2.16.0->web3==6.4.0->rysk-client==0.1.8) (3.3)
+    Requirement already satisfied: markdown-it-py<3.0.0,>=2.1.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rich>=10.7.0->rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (2.2.0)
+    Requirement already satisfied: pygments<3.0.0,>=2.14.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rich>=10.7.0->rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (2.14.0)
+    Requirement already satisfied: pycparser in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cffi>=1.12->cryptography>=2.6.1->ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (2.21)
+    Requirement already satisfied: toolz>=0.8.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cytoolz>=0.10.1->eth-utils>=2.1.0->web3==6.4.0->rysk-client==0.1.8) (0.11.2)
+    Requirement already satisfied: mdurl~=0.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from markdown-it-py<3.0.0,>=2.1.0->rich>=10.7.0->rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (0.1.2)
+    Requirement already satisfied: regex>=2022.3.15 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from parsimonious<0.10.0,>=0.9.0->eth-abi>=4.0.0->web3==6.4.0->rysk-client==0.1.8) (2023.6.3)
+    Building wheels for collected packages: rysk-client
+      Building wheel for rysk-client (pyproject.toml) ... [?25ldone
+    [?25h  Created wheel for rysk-client: filename=rysk_client-0.1.8-py3-none-any.whl size=502097 sha256=b11b92629c38b8e9e13c79cb02a87a28104d78d7262ae3662c364ba00ad48441
+      Stored in directory: /tmp/pip-ephem-wheel-cache-47uzb13y/wheels/85/5d/62/83b40ae2d2c1fc31bec44436912ab30c592085539d92f35254
+    Successfully built rysk-client
     [33mWARNING: Error parsing requirements for vulture: [Errno 2] No such file or directory: '/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/vulture-2.5.dist-info/METADATA'[0m[33m
-    [0m[33mWARNING: You are using pip version 22.0.4; however, version 23.1.2 is available.
+    [0mInstalling collected packages: rysk-client
+      Attempting uninstall: rysk-client
+        Found existing installation: rysk-client 0.1.8
+        Uninstalling rysk-client-0.1.8:
+          Successfully uninstalled rysk-client-0.1.8
+    Successfully installed rysk-client-0.1.8
+    [33mWARNING: You are using pip version 22.0.4; however, version 23.1.2 is available.
     You should consider upgrading via the '/home/tom/.pyenv/versions/3.10.4/bin/python3.10 -m pip install --upgrade pip' command.[0m[33m
     [0m
 
 # Usage
 
 
 
 ```python
 from rysk_client.src.utils import get_web3
 
 web3 = get_web3()
-web3.isConnected()
+web3.is_connected()
 ```
 
 
 
 
     True
 
@@ -92,23 +113,25 @@
 from rysk_client.client import RyskClient
 from tests.conftest import DEFAULT_ADDRESS
 
 auth = {
     "address": DEFAULT_ADDRESS,
 }
 
+print(auth)
+
 client = RyskClient(**auth)
 client
 
 ```
 
 
 
 
-    RyskClient(_markets=[], _tickers=[])
+    RyskClient(_markets=[], _tickers=[], _otokens={})
 
 
 
 ## Fetching Markets
 
 The client can fetch markets as so;
```

### Comparing `rysk_client-0.1.8/pyproject.toml` & `rysk_client-0.1.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "rysk_client"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["8baller <8ball030@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "rysk_client", from = "." },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4"
-web3 = "^5.4.0"
+python = ">=3.8,<4.0"
+web3 = "==6.4.0"
 ccxt = "^3.1.15"
 rich-click = "^1.6.1"
 
 [tool.poetry.group.dev.dependencies]
 autonomy-dev = {extras = ["all"], version = "^0.1.4"}
 jupyterlab = "^4.0.1"
 types-requests = "^2.31.0.1"
```

### Comparing `rysk_client-0.1.8/rysk_client/contracts/Accounting.sol/Accounting.json` & `rysk_client-0.1.9/rysk_client/contracts/Accounting.sol/Accounting.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/AlphaOptionHandler.sol/AlphaOptionHandler.json` & `rysk_client-0.1.9/rysk_client/contracts/AlphaOptionHandler.sol/AlphaOptionHandler.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/AlphaPortfolioValuesFeed.sol/AlphaPortfolioValuesFeed.json` & `rysk_client-0.1.9/rysk_client/contracts/AlphaPortfolioValuesFeed.sol/AlphaPortfolioValuesFeed.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/Authority.sol/Authority.json` & `rysk_client-0.1.9/rysk_client/contracts/Authority.sol/Authority.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/BeyondPricer.sol/BeyondPricer.json` & `rysk_client-0.1.9/rysk_client/contracts/BeyondPricer.sol/BeyondPricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/LiquidityPool.sol/LiquidityPool.json` & `rysk_client-0.1.9/rysk_client/contracts/LiquidityPool.sol/LiquidityPool.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/Manager.sol/Manager.json` & `rysk_client-0.1.9/rysk_client/contracts/Manager.sol/Manager.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/OptionCatalogue.sol/OptionCatalogue.json` & `rysk_client-0.1.9/rysk_client/contracts/OptionCatalogue.sol/OptionCatalogue.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/OptionExchange.sol/OptionExchange.json` & `rysk_client-0.1.9/rysk_client/contracts/OptionExchange.sol/OptionExchange.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/OptionRegistry.sol/OptionRegistry.json` & `rysk_client-0.1.9/rysk_client/contracts/OptionRegistry.sol/OptionRegistry.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/PriceFeed.sol/PriceFeed.json` & `rysk_client-0.1.9/rysk_client/contracts/PriceFeed.sol/PriceFeed.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/Protocol.sol/Protocol.json` & `rysk_client-0.1.9/rysk_client/contracts/Protocol.sol/Protocol.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/VolatilityFeed.sol/VolatilityFeed.json` & `rysk_client-0.1.9/rysk_client/contracts/VolatilityFeed.sol/VolatilityFeed.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/gelato/OpynPricerResolver.sol/OpynPricerResolver.json` & `rysk_client-0.1.9/rysk_client/contracts/gelato/OpynPricerResolver.sol/OpynPricerResolver.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/gelato/VaultCollateralMulticall.sol/VaultCollateralMulticall.json` & `rysk_client-0.1.9/rysk_client/contracts/gelato/VaultCollateralMulticall.sol/VaultCollateralMulticall.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/hedging/GmxHedgingReactor.sol/GmxHedgingReactor.json` & `rysk_client-0.1.9/rysk_client/contracts/hedging/GmxHedgingReactor.sol/GmxHedgingReactor.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/hedging/PerpHedgingReactor.sol/PerpHedgingReactor.json` & `rysk_client-0.1.9/rysk_client/contracts/hedging/PerpHedgingReactor.sol/PerpHedgingReactor.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/hedging/UniswapV3HedgingReactor.sol/UniswapV3HedgingReactor.json` & `rysk_client-0.1.9/rysk_client/contracts/hedging/UniswapV3HedgingReactor.sol/UniswapV3HedgingReactor.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/hedging/UniswapV3RangeOrderReactor.sol/UniswapV3RangeOrderReactor.json` & `rysk_client-0.1.9/rysk_client/contracts/hedging/UniswapV3RangeOrderReactor.sol/UniswapV3RangeOrderReactor.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/AddressBookInterface.sol/AddressBookInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/AddressBookInterface.sol/AddressBookInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/AggregatorInterface.sol/AggregatorInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/AggregatorInterface.sol/AggregatorInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/AggregatorV3Interface.sol/AggregatorV3Interface.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/AggregatorV3Interface.sol/AggregatorV3Interface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/GammaTypes.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/GammaTypes.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/IController.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/IController.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/IOtoken.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/IOtoken.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/GammaInterface.sol/IOtokenFactory.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/GammaInterface.sol/IOtokenFactory.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IAccounting.sol/IAccounting.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IAccounting.sol/IAccounting.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IAlphaOptionHandler.sol/IAlphaOptionHandler.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IAlphaOptionHandler.sol/IAlphaOptionHandler.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IAlphaPortfolioValuesFeed.sol/IAlphaPortfolioValuesFeed.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IAlphaPortfolioValuesFeed.sol/IAlphaPortfolioValuesFeed.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IAuthority.sol/IAuthority.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IAuthority.sol/IAuthority.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IChainlinkPricer.sol/IChainlinkPricer.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IChainlinkPricer.sol/IChainlinkPricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IGmxVault.sol/IGmxVault.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IGmxVault.sol/IGmxVault.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IGmxVaultPriceFeed.sol/IVaultPriceFeed.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IGmxVaultPriceFeed.sol/IVaultPriceFeed.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IHedgingReactor.sol/IHedgingReactor.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IHedgingReactor.sol/IHedgingReactor.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/ILiquidityPool.sol/ILiquidityPool.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/ILiquidityPool.sol/ILiquidityPool.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IMarginCalculator.sol/IMarginCalculator.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IMarginCalculator.sol/IMarginCalculator.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IOptionRegistry.sol/IOptionRegistry.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IOptionRegistry.sol/IOptionRegistry.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IOracle.sol/IOracle.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IOracle.sol/IOracle.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IPortfolioValuesFeed.sol/IPortfolioValuesFeed.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IPortfolioValuesFeed.sol/IPortfolioValuesFeed.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IPositionRouter.sol/IPositionRouter.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IPositionRouter.sol/IPositionRouter.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IPriceFeedTimelock.sol/IPriceFeedTimelock.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IPriceFeedTimelock.sol/IPriceFeedTimelock.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IReader.sol/IReader.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IReader.sol/IReader.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IRouter.sol/IRouter.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IRouter.sol/IRouter.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/IWhitelist.sol/IWhitelist.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/IWhitelist.sol/IWhitelist.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/I_ERC20.sol/I_ERC20.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/I_ERC20.sol/I_ERC20.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/OtokenInterface.sol/OtokenInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/OtokenInterface.sol/OtokenInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/interfaces/WETH.sol/WETH.json` & `rysk_client-0.1.9/rysk_client/contracts/interfaces/WETH.sol/WETH.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/lens/DHVLensMK1.sol/DHVLensMK1.json` & `rysk_client-0.1.9/rysk_client/contracts/lens/DHVLensMK1.sol/DHVLensMK1.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/AccessControl.sol/AccessControl.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/AccessControl.sol/AccessControl.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/BlackScholes.sol/BlackScholes.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/BlackScholes.sol/BlackScholes.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/CombinedActions.sol/CombinedActions.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/CombinedActions.sol/CombinedActions.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/CustomErrors.sol/CustomErrors.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/CustomErrors.sol/CustomErrors.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/EnumerableSet.sol/EnumerableSet.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/EnumerableSet.sol/EnumerableSet.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/NormalDist.sol/NormalDist.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/NormalDist.sol/NormalDist.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/OptionsCompute.sol/OptionsCompute.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/OptionsCompute.sol/OptionsCompute.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/OpynInteractions.sol/OpynInteractions.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/OpynInteractions.sol/OpynInteractions.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/RyskActions.sol/RyskActions.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/RyskActions.sol/RyskActions.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/SABR.sol/SABR.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/SABR.sol/SABR.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/SafeTransferLib.sol/SafeTransferLib.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/SafeTransferLib.sol/SafeTransferLib.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/libraries/Types.sol/Types.json` & `rysk_client-0.1.9/rysk_client/contracts/libraries/Types.sol/Types.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/mocks/ForceSend.sol/ForceSend.json` & `rysk_client-0.1.9/rysk_client/contracts/mocks/ForceSend.sol/ForceSend.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/mocks/MockChainlinkAggregator.sol/MockChainlinkAggregator.json` & `rysk_client-0.1.9/rysk_client/contracts/mocks/MockChainlinkAggregator.sol/MockChainlinkAggregator.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/mocks/MockChainlinkSequencerFeed.sol/MockChainlinkSequencerFeed.json` & `rysk_client-0.1.9/rysk_client/contracts/mocks/MockChainlinkSequencerFeed.sol/MockChainlinkSequencerFeed.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/mocks/MockPortfolioValuesFeed.sol/MockPortfolioValuesFeed.json` & `rysk_client-0.1.9/rysk_client/contracts/mocks/MockPortfolioValuesFeed.sol/MockPortfolioValuesFeed.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/Migrations.sol/Migrations.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/Migrations.sol/Migrations.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/AddressBook.sol/AddressBook.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/AddressBook.sol/AddressBook.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Controller.sol/Controller.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Controller.sol/Controller.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/MarginCalculator.sol/MarginCalculator.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/MarginCalculator.sol/MarginCalculator.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/MarginPool.sol/MarginPool.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/MarginPool.sol/MarginPool.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Oracle.sol/Oracle.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Oracle.sol/Oracle.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Otoken.sol/Otoken.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Otoken.sol/Otoken.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/OtokenFactory.sol/OtokenFactory.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/OtokenFactory.sol/OtokenFactory.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/OtokenSpawner.sol/OtokenSpawner.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/OtokenSpawner.sol/OtokenSpawner.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/core/Whitelist.sol/Whitelist.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/core/Whitelist.sol/Whitelist.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/external/callees/PermitCallee.sol/PermitCallee.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/external/callees/PermitCallee.sol/PermitCallee.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/external/canonical-weth/WETH9.sol/WETH9.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/external/canonical-weth/WETH9.sol/WETH9.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/external/proxies/PayableProxyController.sol/PayableProxyController.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/external/proxies/PayableProxyController.sol/PayableProxyController.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/AddressBookInterface.sol/AddressBookInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/AddressBookInterface.sol/AddressBookInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/AggregatorInterface.sol/AggregatorInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/AggregatorInterface.sol/AggregatorInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/CTokenInterface.sol/CTokenInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/CTokenInterface.sol/CTokenInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/CalleeInterface.sol/CalleeInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/CalleeInterface.sol/CalleeInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/ERC20Interface.sol/ERC20Interface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/ERC20Interface.sol/ERC20Interface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/MarginCalculatorInterface.sol/MarginCalculatorInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/MarginCalculatorInterface.sol/MarginCalculatorInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/MarginPoolInterface.sol/MarginPoolInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/MarginPoolInterface.sol/MarginPoolInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/OpynPricerInterface.sol/OpynPricerInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/OpynPricerInterface.sol/OpynPricerInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/OracleInterface.sol/OracleInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/OracleInterface.sol/OracleInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/OtokenInterface.sol/OtokenInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/OtokenInterface.sol/OtokenInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/WETH9Interface.sol/WETH9Interface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/WETH9Interface.sol/WETH9Interface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/WSTETHInterface.sol/WSTETHInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/WSTETHInterface.sol/WSTETHInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/WhitelistInterface.sol/WhitelistInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/WhitelistInterface.sol/WhitelistInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/YearnVaultInterface.sol/YearnVaultInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/YearnVaultInterface.sol/YearnVaultInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/interfaces/ZeroXExchangeInterface.sol/ZeroXExchangeInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/interfaces/ZeroXExchangeInterface.sol/ZeroXExchangeInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/Actions.sol/Actions.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/Actions.sol/Actions.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/FixedPointInt256.sol/FixedPointInt256.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/FixedPointInt256.sol/FixedPointInt256.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/MarginVault.sol/MarginVault.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/MarginVault.sol/MarginVault.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/libs/SignedConverter.sol/SignedConverter.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/libs/SignedConverter.sol/SignedConverter.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewCalculator.sol/NewMarginCalculator.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewCalculator.sol/NewMarginCalculator.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewController.sol/NewController.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewController.sol/NewController.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewMarginCalculatorInterface.sol/MarginCalculatorInterface.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewMarginCalculatorInterface.sol/MarginCalculatorInterface.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/new/NewWhitelist.sol/NewWhitelist.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/new/NewWhitelist.sol/NewWhitelist.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/BokkyPooBahsDateTimeLibrary.sol/BokkyPooBahsDateTimeLibrary.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/BokkyPooBahsDateTimeLibrary.sol/BokkyPooBahsDateTimeLibrary.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/Spawn.sol/Spawn.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/Spawn.sol/Spawn.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Address.sol/Address.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Address.sol/Address.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Create2.sol/Create2.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Create2.sol/Create2.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/IERC20.sol/IERC20.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/IERC20.sol/IERC20.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Ownable.sol/Ownable.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Ownable.sol/Ownable.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/SafeERC20.sol/SafeERC20.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/SafeERC20.sol/SafeERC20.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/SafeMath.sol/SafeMath.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/SafeMath.sol/SafeMath.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/SignedSafeMath.sol/SignedSafeMath.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/SignedSafeMath.sol/SignedSafeMath.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/Strings.sol/Strings.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/Strings.sol/Strings.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ERC20Upgradeable.sol/ERC20Upgradeable.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ERC20Upgradeable.sol/ERC20Upgradeable.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/IERC20Upgradeable.sol/IERC20Upgradeable.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/IERC20Upgradeable.sol/IERC20Upgradeable.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Initializable.sol/Initializable.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Initializable.sol/Initializable.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnableUpgradeSafe.sol/OwnableUpgradeSafe.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnableUpgradeSafe.sol/OwnableUpgradeSafe.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnedUpgradeabilityProxy.sol/OwnedUpgradeabilityProxy.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnedUpgradeabilityProxy.sol/OwnedUpgradeabilityProxy.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Proxy.sol/Proxy.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Proxy.sol/Proxy.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ReentrancyGuardUpgradeSafe.sol/ReentrancyGuardUpgradeSafe.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ReentrancyGuardUpgradeSafe.sol/ReentrancyGuardUpgradeSafe.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/UpgradeabilityProxy.sol/UpgradeabilityProxy.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/UpgradeabilityProxy.sol/UpgradeabilityProxy.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/cryptography/ECDSAUpgradeable.sol/ECDSAUpgradeable.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/cryptography/ECDSAUpgradeable.sol/ECDSAUpgradeable.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/ERC20PermitUpgradeable.sol/ERC20PermitUpgradeable.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/ERC20PermitUpgradeable.sol/ERC20PermitUpgradeable.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/math/SafeMathUpgradeable.sol/SafeMathUpgradeable.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/math/SafeMathUpgradeable.sol/SafeMathUpgradeable.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/utils/CountersUpgradeable.sol/CountersUpgradeable.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/utils/CountersUpgradeable.sol/CountersUpgradeable.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/ChainlinkPricer.sol/ChainLinkPricer.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/ChainlinkPricer.sol/ChainLinkPricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/CompoundPricer.sol/CompoundPricer.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/CompoundPricer.sol/CompoundPricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/WstethPricer.sol/WstethPricer.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/WstethPricer.sol/WstethPricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/packages/opyn/pricers/YearnPricer.sol/YearnPricer.json` & `rysk_client-0.1.9/rysk_client/contracts/packages/opyn/pricers/YearnPricer.sol/YearnPricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/tokens/ERC20.sol/ERC20.json` & `rysk_client-0.1.9/rysk_client/contracts/tokens/ERC20.sol/ERC20.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/tokens/MintableERC20.sol/MintableERC20.json` & `rysk_client-0.1.9/rysk_client/contracts/tokens/MintableERC20.sol/MintableERC20.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/tokens/WETH.sol/WETH.json` & `rysk_client-0.1.9/rysk_client/contracts/tokens/WETH.sol/WETH.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholes.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholes.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholesTest.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholesTest.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/BlackScholesTest.sol/NormalDist.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/BlackScholesTest.sol/NormalDist.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/LiquidityPoolAdjustCollateralTest.sol/LiquidityPoolAdjustCollateralTest.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/LiquidityPoolAdjustCollateralTest.sol/LiquidityPoolAdjustCollateralTest.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/OracleMock.sol/OracleMock.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/OracleMock.sol/OracleMock.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/PerpHedgingTest.sol/PerpHedgingTest.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/PerpHedgingTest.sol/PerpHedgingTest.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/RealTokenMock.sol/RealTokenMock.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/RealTokenMock.sol/RealTokenMock.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/ReentrancyGuard.sol/ReentrancyGuard.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/ReentrancyGuard.sol/ReentrancyGuard.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/UniswapConversionsTest.sol/UniswapConversionsTest.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/UniswapConversionsTest.sol/UniswapConversionsTest.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/UniswapV3HedgingTest.sol/UniswapV3HedgingTest.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/UniswapV3HedgingTest.sol/UniswapV3HedgingTest.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/utils/Volatility.sol/Volatility.json` & `rysk_client-0.1.9/rysk_client/contracts/utils/Volatility.sol/Volatility.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/FullMath.sol/FullMath.json` & `rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/FullMath.sol/FullMath.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/LiquidityAmounts.sol/LiquidityAmounts.json` & `rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/LiquidityAmounts.sol/LiquidityAmounts.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/PoolAddress.sol/PoolAddress.json` & `rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/PoolAddress.sol/PoolAddress.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/contracts/vendor/uniswap/TickMath.sol/TickMath.json` & `rysk_client-0.1.9/rysk_client/contracts/vendor/uniswap/TickMath.sol/TickMath.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/src/collateral.py` & `rysk_client-0.1.9/rysk_client/src/collateral.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from web3 import Web3
 
 
 class Collateral(Enum):
     """Collateral supported by the protocol"""
 
-    WETH = Web3.toChecksumAddress("0x3b3a1de07439eeb04492fa64a889ee25a130cdd3")
-    USDC = Web3.toChecksumAddress("0x408c5755b5c7a0a28d851558ea3636cfc5b5b19d")
+    WETH = Web3.to_checksum_address("0x3b3a1de07439eeb04492fa64a889ee25a130cdd3")
+    USDC = Web3.to_checksum_address("0x408c5755b5c7a0a28d851558ea3636cfc5b5b19d")
 
     @classmethod
     def is_supported(cls, collateral):
         """Is the sset supported"""
         try:
             cls.from_symbol(collateral)
         except ValueError:
```

### Comparing `rysk_client-0.1.8/rysk_client/src/position.py` & `rysk_client-0.1.9/rysk_client/src/position.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,30 @@
 class OrderSide(Enum):
     """Enum to represent the side of an order."""
 
     BUY = "buy"
     SELL = "sell"
 
 
+@dataclass
 class Order:
     """Class to represent an order"""
 
     price: float
     amount: float
     order_id: str
     order_side: OrderSide
     order_type: str = "market"
 
+    def __str__(self) -> str:
+        return f"Order({self.order_side}, {self.amount}, {self.price})"
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
 
 class PositionSide(Enum):
     """Enum to represent the side of a position."""
 
     LONG = "long"
     SHORT = "short"
```

### Comparing `rysk_client-0.1.8/rysk_client/src/subgraph.py` & `rysk_client-0.1.9/rysk_client/src/subgraph.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/rysk_client/src/utils.py` & `rysk_client-0.1.9/rysk_client/src/utils.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.1.8/PKG-INFO` & `rysk_client-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,100 +1,121 @@
 Metadata-Version: 2.1
 Name: rysk-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: 8baller
 Author-email: 8ball030@gmail.com
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ccxt (>=3.1.15,<4.0.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
-Requires-Dist: web3 (>=5.4.0,<6.0.0)
+Requires-Dist: web3 (==6.4.0)
 Description-Content-Type: text/markdown
 
 # Rysk Client
 
 ## Installation
 
-### Dev
+The application is availale on pypi and can be installed as so;
 
-dependencies are managed with poetry. 
+    ```bash
+    pip install rysk-client
+    ```
+
+### Dev & Contributing
+
+Dependencies are managed with poetry.
 
 For dev build.
 
 
 ```python
-!pip install rysk-client
+!pip install -U .
 ```
 
-    Requirement already satisfied: rysk-client in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (0.1.3)
-    Requirement already satisfied: web3<6.0.0,>=5.4.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client) (5.25.0)
-    Requirement already satisfied: ccxt<4.0.0,>=3.1.15 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client) (3.1.17)
-    Requirement already satisfied: requests>=2.18.4 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (2.28.1)
-    Requirement already satisfied: cryptography>=2.6.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (39.0.1)
-    Requirement already satisfied: setuptools>=60.9.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (67.8.0)
-    Requirement already satisfied: aiodns>=1.1.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (3.0.0)
-    Requirement already satisfied: certifi>=2018.1.18 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (2022.6.15)
-    Requirement already satisfied: aiohttp>=3.8 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (3.8.4)
-    Requirement already satisfied: yarl>=1.7.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client) (1.7.2)
-    Requirement already satisfied: protobuf<4,>=3.10.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (3.20.3)
-    Requirement already satisfied: eth-typing<3.0.0,>=2.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (2.3.0)
-    Requirement already satisfied: hexbytes<1.0.0,>=0.1.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (0.3.0)
-    Requirement already satisfied: eth-utils<2.0.0,>=1.9.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (1.9.5)
-    Requirement already satisfied: websockets<10,>=9.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (9.1)
-    Requirement already satisfied: lru-dict<2.0.0,>=1.1.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (1.1.8)
-    Requirement already satisfied: eth-account<0.6.0,>=0.5.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (0.5.6)
-    Requirement already satisfied: eth-hash[pycryptodome]<1.0.0,>=0.2.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (0.5.0)
-    Requirement already satisfied: ipfshttpclient==0.8.0a2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (0.8.0a2)
-    Requirement already satisfied: jsonschema<4.0.0,>=3.2.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (3.2.0)
-    Requirement already satisfied: eth-abi<3.0.0,>=2.0.0b6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3<6.0.0,>=5.4.0->rysk-client) (2.2.0)
-    Requirement already satisfied: multiaddr>=0.0.7 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ipfshttpclient==0.8.0a2->web3<6.0.0,>=5.4.0->rysk-client) (0.0.9)
-    Requirement already satisfied: pycares>=4.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiodns>=1.1.1->ccxt<4.0.0,>=3.1.15->rysk-client) (4.2.2)
-    Requirement already satisfied: multidict<7.0,>=4.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (6.0.2)
-    Requirement already satisfied: async-timeout<5.0,>=4.0.0a3 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (4.0.2)
-    Requirement already satisfied: attrs>=17.3.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (22.1.0)
-    Requirement already satisfied: charset-normalizer<4.0,>=2.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (2.1.1)
-    Requirement already satisfied: frozenlist>=1.1.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (1.3.1)
-    Requirement already satisfied: aiosignal>=1.1.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.8->ccxt<4.0.0,>=3.1.15->rysk-client) (1.2.0)
-    Requirement already satisfied: cffi>=1.12 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cryptography>=2.6.1->ccxt<4.0.0,>=3.1.15->rysk-client) (1.15.1)
-    Requirement already satisfied: parsimonious<0.9.0,>=0.8.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-abi<3.0.0,>=2.0.0b6->web3<6.0.0,>=5.4.0->rysk-client) (0.8.1)
-    Requirement already satisfied: rlp<3,>=1.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (2.0.1)
-    Requirement already satisfied: eth-rlp<2,>=0.1.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (0.2.1)
-    Requirement already satisfied: bitarray<1.3.0,>=1.2.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (1.2.2)
-    Requirement already satisfied: eth-keyfile<0.6.0,>=0.5.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (0.5.1)
-    Requirement already satisfied: eth-keys!=0.3.2,<0.4.0,>=0.2.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account<0.6.0,>=0.5.6->web3<6.0.0,>=5.4.0->rysk-client) (0.3.4)
-    Requirement already satisfied: pycryptodome<4,>=3.6.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-hash[pycryptodome]<1.0.0,>=0.2.0->web3<6.0.0,>=5.4.0->rysk-client) (3.15.0)
-    Requirement already satisfied: cytoolz<1.0.0,>=0.10.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-utils<2.0.0,>=1.9.5->web3<6.0.0,>=5.4.0->rysk-client) (0.12.0)
-    Requirement already satisfied: pyrsistent>=0.14.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from jsonschema<4.0.0,>=3.2.0->web3<6.0.0,>=5.4.0->rysk-client) (0.18.1)
-    Requirement already satisfied: six>=1.11.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from jsonschema<4.0.0,>=3.2.0->web3<6.0.0,>=5.4.0->rysk-client) (1.16.0)
-    Requirement already satisfied: idna<4,>=2.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from requests>=2.18.4->ccxt<4.0.0,>=3.1.15->rysk-client) (3.3)
-    Requirement already satisfied: urllib3<1.27,>=1.21.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from requests>=2.18.4->ccxt<4.0.0,>=3.1.15->rysk-client) (1.26.12)
-    Requirement already satisfied: pycparser in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cffi>=1.12->cryptography>=2.6.1->ccxt<4.0.0,>=3.1.15->rysk-client) (2.21)
-    Requirement already satisfied: toolz>=0.8.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cytoolz<1.0.0,>=0.10.1->eth-utils<2.0.0,>=1.9.5->web3<6.0.0,>=5.4.0->rysk-client) (0.11.2)
-    Requirement already satisfied: netaddr in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from multiaddr>=0.0.7->ipfshttpclient==0.8.0a2->web3<6.0.0,>=5.4.0->rysk-client) (0.8.0)
-    Requirement already satisfied: base58 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from multiaddr>=0.0.7->ipfshttpclient==0.8.0a2->web3<6.0.0,>=5.4.0->rysk-client) (2.1.1)
-    Requirement already satisfied: varint in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from multiaddr>=0.0.7->ipfshttpclient==0.8.0a2->web3<6.0.0,>=5.4.0->rysk-client) (1.0.2)
+    Processing /home/tom/Desktop/Fun/rysk_explorations
+      Installing build dependencies ... [?25ldone
+    [?25h  Getting requirements to build wheel ... [?25ldone
+    [?25h  Preparing metadata (pyproject.toml) ... [?25ldone
+    [?25hRequirement already satisfied: web3==6.4.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client==0.1.8) (6.4.0)
+    Requirement already satisfied: ccxt<4.0.0,>=3.1.15 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client==0.1.8) (3.1.17)
+    Requirement already satisfied: rich-click<2.0.0,>=1.6.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rysk-client==0.1.8) (1.6.1)
+    Requirement already satisfied: jsonschema>=4.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (4.17.3)
+    Requirement already satisfied: requests>=2.16.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (2.28.1)
+    Requirement already satisfied: eth-abi>=4.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (4.0.0)
+    Requirement already satisfied: eth-account>=0.8.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (0.9.0)
+    Requirement already satisfied: aiohttp>=3.7.4.post0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (3.8.4)
+    Requirement already satisfied: eth-hash[pycryptodome]>=0.5.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (0.5.2)
+    Requirement already satisfied: hexbytes>=0.1.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (0.3.0)
+    Requirement already satisfied: lru-dict>=1.1.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (1.1.8)
+    Requirement already satisfied: eth-typing>=3.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (3.4.0)
+    Requirement already satisfied: eth-utils>=2.1.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (2.1.1)
+    Requirement already satisfied: protobuf>=4.21.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (4.23.2)
+    Requirement already satisfied: websockets>=10.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from web3==6.4.0->rysk-client==0.1.8) (11.0.3)
+    Requirement already satisfied: cryptography>=2.6.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (39.0.1)
+    Requirement already satisfied: aiodns>=1.1.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (3.0.0)
+    Requirement already satisfied: certifi>=2018.1.18 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (2022.6.15)
+    Requirement already satisfied: yarl>=1.7.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (1.7.2)
+    Requirement already satisfied: setuptools>=60.9.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (67.8.0)
+    Requirement already satisfied: rich>=10.7.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (13.3.1)
+    Requirement already satisfied: click>=7 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (8.0.2)
+    Requirement already satisfied: pycares>=4.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiodns>=1.1.1->ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (4.2.2)
+    Requirement already satisfied: charset-normalizer<4.0,>=2.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (2.1.1)
+    Requirement already satisfied: frozenlist>=1.1.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (1.3.1)
+    Requirement already satisfied: async-timeout<5.0,>=4.0.0a3 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (4.0.2)
+    Requirement already satisfied: aiosignal>=1.1.2 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (1.2.0)
+    Requirement already satisfied: multidict<7.0,>=4.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (6.0.2)
+    Requirement already satisfied: attrs>=17.3.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from aiohttp>=3.7.4.post0->web3==6.4.0->rysk-client==0.1.8) (22.1.0)
+    Requirement already satisfied: cffi>=1.12 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cryptography>=2.6.1->ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (1.15.1)
+    Requirement already satisfied: parsimonious<0.10.0,>=0.9.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-abi>=4.0.0->web3==6.4.0->rysk-client==0.1.8) (0.9.0)
+    Requirement already satisfied: eth-rlp>=0.3.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (0.3.0)
+    Requirement already satisfied: rlp>=1.0.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (3.0.0)
+    Requirement already satisfied: eth-keys>=0.4.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (0.4.0)
+    Requirement already satisfied: eth-keyfile>=0.6.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (0.6.1)
+    Requirement already satisfied: bitarray>=2.4.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-account>=0.8.0->web3==6.4.0->rysk-client==0.1.8) (2.7.4)
+    Requirement already satisfied: pycryptodome<4,>=3.6.6 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-hash[pycryptodome]>=0.5.1->web3==6.4.0->rysk-client==0.1.8) (3.15.0)
+    Requirement already satisfied: cytoolz>=0.10.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from eth-utils>=2.1.0->web3==6.4.0->rysk-client==0.1.8) (0.12.0)
+    Requirement already satisfied: pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from jsonschema>=4.0.0->web3==6.4.0->rysk-client==0.1.8) (0.18.1)
+    Requirement already satisfied: urllib3<1.27,>=1.21.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from requests>=2.16.0->web3==6.4.0->rysk-client==0.1.8) (1.26.12)
+    Requirement already satisfied: idna<4,>=2.5 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from requests>=2.16.0->web3==6.4.0->rysk-client==0.1.8) (3.3)
+    Requirement already satisfied: markdown-it-py<3.0.0,>=2.1.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rich>=10.7.0->rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (2.2.0)
+    Requirement already satisfied: pygments<3.0.0,>=2.14.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from rich>=10.7.0->rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (2.14.0)
+    Requirement already satisfied: pycparser in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cffi>=1.12->cryptography>=2.6.1->ccxt<4.0.0,>=3.1.15->rysk-client==0.1.8) (2.21)
+    Requirement already satisfied: toolz>=0.8.0 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from cytoolz>=0.10.1->eth-utils>=2.1.0->web3==6.4.0->rysk-client==0.1.8) (0.11.2)
+    Requirement already satisfied: mdurl~=0.1 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from markdown-it-py<3.0.0,>=2.1.0->rich>=10.7.0->rich-click<2.0.0,>=1.6.1->rysk-client==0.1.8) (0.1.2)
+    Requirement already satisfied: regex>=2022.3.15 in /home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages (from parsimonious<0.10.0,>=0.9.0->eth-abi>=4.0.0->web3==6.4.0->rysk-client==0.1.8) (2023.6.3)
+    Building wheels for collected packages: rysk-client
+      Building wheel for rysk-client (pyproject.toml) ... [?25ldone
+    [?25h  Created wheel for rysk-client: filename=rysk_client-0.1.8-py3-none-any.whl size=502097 sha256=b11b92629c38b8e9e13c79cb02a87a28104d78d7262ae3662c364ba00ad48441
+      Stored in directory: /tmp/pip-ephem-wheel-cache-47uzb13y/wheels/85/5d/62/83b40ae2d2c1fc31bec44436912ab30c592085539d92f35254
+    Successfully built rysk-client
     [33mWARNING: Error parsing requirements for vulture: [Errno 2] No such file or directory: '/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/vulture-2.5.dist-info/METADATA'[0m[33m
-    [0m[33mWARNING: You are using pip version 22.0.4; however, version 23.1.2 is available.
+    [0mInstalling collected packages: rysk-client
+      Attempting uninstall: rysk-client
+        Found existing installation: rysk-client 0.1.8
+        Uninstalling rysk-client-0.1.8:
+          Successfully uninstalled rysk-client-0.1.8
+    Successfully installed rysk-client-0.1.8
+    [33mWARNING: You are using pip version 22.0.4; however, version 23.1.2 is available.
     You should consider upgrading via the '/home/tom/.pyenv/versions/3.10.4/bin/python3.10 -m pip install --upgrade pip' command.[0m[33m
     [0m
 
 # Usage
 
 
 
 ```python
 from rysk_client.src.utils import get_web3
 
 web3 = get_web3()
-web3.isConnected()
+web3.is_connected()
 ```
 
 
 
 
     True
 
@@ -109,23 +130,25 @@
 from rysk_client.client import RyskClient
 from tests.conftest import DEFAULT_ADDRESS
 
 auth = {
     "address": DEFAULT_ADDRESS,
 }
 
+print(auth)
+
 client = RyskClient(**auth)
 client
 
 ```
 
 
 
 
-    RyskClient(_markets=[], _tickers=[])
+    RyskClient(_markets=[], _tickers=[], _otokens={})
 
 
 
 ## Fetching Markets
 
 The client can fetch markets as so;
```

