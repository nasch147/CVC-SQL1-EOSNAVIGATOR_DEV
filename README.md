# CVC-SQL1-EOSNAVIGATOR_DEV

Server\instance: CVC-SQL1\EOSNAVIGATOR_DEV
Database: Navigator
Tables: 
Staging.CVC ContractInformationData
Staging.CVC_JobInfoData
Staging.CVC_LegalData
Staging.CVC_JobSpecData
Staging.CVC_JobCostData

Below 3 tables doesn't have any data in the DB tables.

Staging.CVC_LegalData
Staging.CVC_JobSpecData
Staging.CVC_JobCostData

[Staging].[CVC_ContractInformationData](
[PK] [int] IDENTITY(1,1) NOT NULL,
[CVC_ContractInformation_PK] [int] NOT NULL,
[Estimate_PK] [int] NOT NULL,
[CompanyID] [varchar](2) NULL,
[DivisionID] [varchar](2) NULL,
[BuilderID] [varchar](2) NULL,
[ProjectName] [varchar](100) NULL,
[CustomerID] [varchar](5) NULL,
[JobNo] [varchar](6) NULL,
[SubJobNo] [varchar](3) NULL,
[Contract] [varchar](1) NULL,
[ItemNumber] [varchar](15) NULL,
[Plan] [varchar](20) NULL,
[Address] [varchar](20) NULL,
[EffectiveDate] [varchar](8) NULL,
[ContractAmount] [decimal](12, 2) NULL,
[Quantity] [decimal](13, 2) NULL,
[Unit] [varchar](2) NULL,
[UnitPrice] [decimal](9, 2) NULL,
[JCDistributionSubJob] [varchar](6) NULL,
[JCDistribution] [varchar](15) NULL,
[JCDistributionCostType] [varchar](1) NULL,
[JCDistributionRecordType] [int] NULL,
[FixedContract] [bit] NULL,
[IncludeInMarkup] [bit] NULL,
[TaxCode1] [varchar](1) NULL,
[TaxCode2] [varchar](1) NULL,
[TaxCode3] [varchar](1) NULL,
[PublishBy] [varchar](100) NULL,
[PublishDate] [datetime] NULL,

[Staging].[CVC_JobCostData](
[PK] [int] IDENTITY(1,1) NOT NULL,
[Estimate_PK] [int] NOT NULL,
[CompanyID] [varchar](2) NULL,
[DivisionID] [varchar](2) NULL,
[JobNo] [varchar](6) NULL,
[SubJobNo] [varchar](3) NULL,
[CostCode] [varchar](15) NULL,
[CostType] [varchar](1) NULL,
[Quantity] [decimal](7, 2) NULL,
[QuantityBare] [decimal](7, 2) NULL,
[Unit] [varchar](2) NULL,
[Hours] [decimal](13, 2) NULL,
[Amount] [decimal](11, 2) NULL,
[PublishBy] [varchar](100) NULL,
[PublishDate] [datetime] NULL,

[Staging].[CVC_JobInfoData](
[PK] [int] IDENTITY(1,1) NOT NULL,
[Estimate_PK] [int] NOT NULL,
[CompanyID] [varchar](2) NULL,
[DivisionID] [varchar](2) NULL,
[JobNo] [varchar](6) NULL,
[SubJobNo] [varchar](3) NULL,
[FoundationSlabEdge] [varchar](10) NULL,
[FoundationFootingSize] [varchar](10) NULL,
[FoundationFootingRebar] [varchar](10) NULL,
[FoundationFootingDowel] [varchar](10) NULL,
[FoundationFootingWC] [varchar](10) NULL,
[FoundationFootingPSI] [varchar](10) NULL,
[FoundationSlabThickness] [varchar](10) NULL,
[FoundationSlabReinforcement] [varchar](10) NULL,
[FoundationRocksandThickness] [varchar](10) NULL,
[FoundationUpperBaseThickness] [varchar](10) NULL,
[FoundationUpperBaseType] [varchar](10) NULL,
[FoundationLowerBaseThickness] [varchar](10) NULL,
[FoundationLowerBaseType] [varchar](10) NULL,
[FoundationVapoRetarder] [varchar](10) NULL,
[FoundationWCRatio] [varchar](10) NULL,
[FoundationPSI] [varchar](10) NULL,
[FoundationContractName] [varchar](10) NULL,
[FoundationContractDate] [varchar](10) NULL,
[FoundationContractPricingPending] [varchar](10) NULL,
[FoundationContractSOWPending] [varchar](10) NULL,
[FoundationContractInsurancePending] [varchar](10) NULL,
[FoundationContractNotesPending] [varchar](10) NULL,
[FoundationProposal] [varchar](10) NULL,
[FoundationBudget] [varchar](10) NULL,
[FoundationLatestPlanLink] [varchar](10) NULL,
[FoundationTaxRate] [varchar](10) NULL,
[FoundationEquipment] [varchar](10) NULL,
[FoundationGLInsurance] [varchar](10) NULL,
[FoundationBudgetMargin] [varchar](10) NULL,
[FoundationOverallLotCount] [varchar](10) NULL,
[FoundationOutOfLevel] [varchar](10) NULL,
[FoundationDeepenedFooting] [varchar](10) NULL,
[FoundationWalls] [varchar](10) NULL,
[FoundationCurrentConcreteQuote] [varchar](10) NULL,
[FoundationConcreteQuoteDate] [varchar](10) NULL,
[FoundationConreteIncreaseDate] [varchar](10) NULL,
[FoundationMixDesignNo] [varchar](10) NULL,
[FlatworkMixDesignNo] [varchar](10) NULL,
[PublishBy] [varchar](100) NULL,
[PublishDate] [datetime] NULL,

[Staging].[CVC_JobSpecData](
[PK] [int] IDENTITY(1,1) NOT NULL,
[Estimate_PK] [int] NOT NULL,
[CompanyID] [varchar](2) NULL,
[DivisionID] [varchar](2) NULL,
[JobNo] [varchar](6) NULL,
[SubJobNo] [varchar](3) NULL,
[FoundationSlabEdge] [varchar](10) NULL,
[FoundationFootingSize] [varchar](10) NULL,
[FoundationFootingRebar] [varchar](10) NULL,
[FoundationFootingDowel] [varchar](10) NULL,
[FoundationFootingWC] [varchar](10) NULL,
[FoundationFootingPSI] [varchar](10) NULL,
[FoundationSlabThickness] [varchar](10) NULL,
[FoundationSlabReinforcement] [varchar](10) NULL,
[FoundationRocksandThickness] [varchar](10) NULL,
[FoundationUpperBaseThickness] [varchar](10) NULL,
[FoundationUpperBaseType] [varchar](50) NULL,
[FoundationLowerBaseThickness] [varchar](10) NULL,
[FoundationLowerBaseType] [varchar](50) NULL,
[FoundationVaporRetarder] [varchar](50) NULL,
[FoundationWCRatio] [varchar](10) NULL,
[FoundationPSI] [varchar](10) NULL,
[FoundationContractName] [varchar](10) NULL,
[FoundationContractDate] [datetime] NULL,
[FoundationContractPricingPending] [bit] NULL,
[FoundationContractSOWPending] [bit] NULL,
[FoundationContractInsurancePending] [bit] NULL,
[FoundationContractNotesPending] [bit] NULL,
[FoundationProposal] [decimal](28, 4) NULL,
[FoundationBudget] [decimal](28, 4) NULL,
[FoundationLatestPlanLink] [varchar](100) NULL,
[FoundationTaxRate] [decimal](28, 4) NULL,
[FoundationEquipment] [decimal](28, 4) NULL,
[FoundationGLInsurance] [decimal](28, 4) NULL,
[FoundationBudgetMargin] [decimal](28, 4) NULL,
[FoundationOverallLotCount] [int] NULL,
[FoundationOutOfLevel] [bit] NULL,
[FoundationDeepenedFooting] [bit] NULL,
[FoundationWalls] [bit] NULL,
[FoundationCurrentConcreteQuote] [decimal](28, 4) NULL,
[FoundationConcreteQuoteDate] [datetime] NULL,
[FoundationConreteIncreaseDate] [datetime] NULL,
[FoundationMixDesignNo] [varchar](50) NULL,
[FlatworkMixDesignNo] [varchar](50) NULL,
[PublishBy] [varchar](100) NULL,
[PublishDate] [datetime] NULL,

[Staging].[CVC_LegalData](
[PK] [int] IDENTITY(1,1) NOT NULL,
[Estimate_PK] [int] NOT NULL,
[CompanyID] [varchar](2) NULL,
[DivisionID] [varchar](2) NULL,
[JobNo] [varchar](6) NULL,
[ContractRevision] [varchar](6) NULL,
[Owner] [varchar](100) NULL,
[Contractor] [varchar](100) NULL,
[Subcontractor] [varchar](20) NULL,
[ContractDate] [datetime] NULL,
[Version] [varchar](20) NULL,
[Lender] [varchar](100) NULL,
[ContractType] [varchar](20) NULL,
[LiquidatedDamages] [decimal](28, 4) NULL,
[TerminationTerms] [varchar](20) NULL,
[TerminationPay] [varchar](100) NULL,
[WarrantyPeriod] [int] NULL,
[NoticeDays] [int] NULL,
[PermittedDelays] [varchar](20) NULL,
[StartDate] [datetime] NULL,
[BondAmount] [decimal](28, 4) NULL,
[BondRequired] [varchar](20) NULL,
[DateReceived] [datetime] NULL,
[BondAgentNotified] [varchar](100) NULL,
[LegalReviewDate] [datetime] NULL,
[ScopeReviewDate] [datetime] NULL,
[CommentsSentDate] [datetime] NULL,
[CommentsResponseDate] [datetime] NULL,
[ContractExecutedDate] [datetime] NULL,
[ContractStatus] [varchar](20) NULL,
[InsuranceStatus] [bit] NULL,
[OpsContactPerson] [varchar](100) NULL,
[APContactPerson] [varchar](100) NULL,
[ContactNumber] [varchar](100) NULL,
[ContactAddress] [varchar](100) NULL,
[CGLPolicy] [varchar](20) NULL,
[WCPolicy] [varchar](20) NULL,
[AutoPolicy] [varchar](20) NULL,
[ExcessPolicy] [varchar](20) NULL,
[GLOccupancyLimit] [decimal](28, 4) NULL,
[GLAggregateLimit] [decimal](28, 4) NULL,
[GLCompOpLimit] [decimal](28, 4) NULL,
[GLPollution] [bit] NULL,
[CompletedOpsReq] [bit] NULL,
[GLPersInjuryLimit] [decimal](28, 4) NULL,
[GLOccurance/Claim] [varchar](20) NULL,
[GLLimit] [decimal](28, 4) NULL,
[WCBodilyInjuryLimit] [decimal](28, 4) NULL,
[WCDiseaseLimit] [decimal](28, 4) NULL,
[WCAggregateLimit] [decimal](28, 4) NULL,
[WCWaiverofSubrogration] [bit] NULL,
[ALOccuranceLimit] [decimal](28, 4) NULL,
[ALAggregateLimit] [decimal](28, 4) NULL,
[AdditionalInsured] [varchar](100) NULL,
[CertificateHolders] [varchar](100) NULL,
[UmbrellaPolicy] [bit] NULL,
[ExcessPolicyLimit] [decimal](28, 4) NULL,
[ExcellLineBacking] [varchar](20) NULL,
[OCIP] [bit] NULL,
[OCIPCoverage] [varchar](20) NULL,
[OCIPSubDeductible] [decimal](28, 4) NULL,
[OCIPOwnerDeductible] [decimal](28, 4) NULL,
[OCIPDeductibleType] [varchar](20) NULL,
[OCIPTPA] [decimal](28, 4) NULL,
[OCIPBidCredit] [decimal](28, 4) NULL,
[OCIPOccurrenceLimit] [decimal](28, 4) NULL,
[OCIPAggregateLimit] [decimal](28, 4) NULL,
[OCIPExcessLimit] [decimal](28, 4) NULL,
[GLSubAccount] [varchar](20) NULL,
[State] [varchar](20) NULL,
[PrevalingWage] [bit] NULL,
[WageDeterminationReceived] [varchar](20) NULL,
[CertifiedPayroll] [bit] NULL,
[ScheduleofValues] [bit] NULL,
[BillDate] [datetime] NULL,
[PayDate] [datetime] NULL,
[Retention] [decimal](28, 4) NULL,
[BillingInstructions] [bit] NULL,
[AddBillingInstructions] [bit] NULL,
[PublishBy] [varchar](100) NULL,
[PublishDate] [datetime] NULL,
