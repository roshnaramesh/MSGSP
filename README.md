# MSGSP
Mining Sequential Patterns Based on GSP (Generalized Sequential Patterns) MS-GSP algorithm - Sequential pattern mining using multiple minimum supports with a support difference constraint.

Input format:
data.txt:Each line represents a Transaction Sequence and each set in a sequence represents a set of items.

    <{20, 30, 80}{70}{50, 70}>
    <{20, 30}{30, 70, 80}>
    <{20, 40}{70}{20, 30, 70}>
    <{10, 30}{40}>
    <{10, 40, 90}{40, 90}>
    <{10, 40, 70}{40, 90}>

para.txt:Gives the minimum item support for each item as well as the support difference constraint

    MIS(10) = 0.43
    MIS(20) = 0.30
    MIS(30) = 0.30
    MIS(40) = 0.40
    MIS(50) = 0.40
    MIS(60) = 0.30
    MIS(70) = 0.20
    MIS(80) = 0.20
    MIS(90) = 0.20

Support_Diff_Constraint = 0.1

Output format:

    Pattern :<{30,20}{70,80}{20,30,70}> count: 10
