
# Zomato_analysis

### Here, I have used SQL to analyse and answer 12 different questions.
<li> I have created 4 dataset namely users, sales, product and goldusers_signup. </li>
<li> I have given dump values for them </li>
<Li> I got lazy with the formatting, if you can't understand the table just click the link

### These are the questions that I've answered with the output table given below:
1) What is the total amount each customer spent on zomato?

| userid        | total_amt_spent  |
| ------------- | ---------------- |
| 1             | 5230             |
| 2             | 2510             |
| 3             | 4570             |

2) How many days has each customer visited zomato?

| userid        | distinct_days  |
| ------------- | -------------- |
| 1             | 7              |
| 2             | 4              |
| 3             | 5              |

3) What was the first product purchased by each customer?

userid	created_date	product_id	rnk
1	11-03-2016	1	1
2	24-09-2017	1	1
3	10-11-2016	1	1
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/490f3e6c-8afb-4ff5-b484-718b168eb2d2)

4) What is the most purchased item on the menu and how many times was it purchased by all customers?

userid	cnt
1	3
2	1
3	3
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/88aae452-8d15-4c96-be01-d81292a64ccd)

5) Which item was the most popular for each customer?

userid	product_id	cnt	rnk
1	2	3	1
2	3	2	1
3	2	3	1
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/91d5ae30-80ab-4ecf-ae95-403cd52bc4c5)

6) Which item was purchased first by the customer after they became a member?

userid	created_date	product_id	gold_signup_date	rnk
1	19-03-2018	3	22-09-2017	1
3	07-12-2017	2	21-04-2017	1
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/5680df76-aaf4-42e2-ae88-7adc142b8db0)

7) Which item was purchased just before the customer became a member?

userid	created_date	product_id	gold_signup_date	rnk
1	19-04-2017	2	22-09-2017	1
3	20-12-2016	2	21-04-2017	1
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/2ccb4835-5d4c-4790-ae9e-79a54096c732)

8) What is the total orders and amount spent for each member before they became a member?

userid	order_purchased	total_amt_spent
1	05-01-1900	4030
3	03-01-1900	2720
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/4e388c8c-4560-4bfd-a9dd-122a89a20249)

9) If buying each product generates points (eg. 5rs = 2 zomato point) and each product has different purchasing points
eg. for p1 5rs=1 zomato point, for p2 10rs=5 zomato point and p3 5rs=1 zomato point

product_id	total_points_earned	rnk
2	02-05-1908	1
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/1c6a2be4-4840-442e-a8d1-3325a2e773bd)

10) In the first one year after a customer joins the gold program (including their join date) irrespective of what the customer has purchased they earn 5 zomato points for every 10 rs spent who earned more 1 or 3 and what was their points earnings in their first year?

userid	created_date	product_id	gold_signup_date	total_points_earned
1	19-03-2018	3	22-09-2017	165
3	07-12-2017	2	21-04-2017	435
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/2139ddc4-c78b-4c09-be47-f21e753598f4)

11) rnk all the transaction of the customers

userid	created_date	product_id	rnk
1	11-03-2016	1	1
1	20-05-2016	3	2
1	09-11-2016	1	3
1	11-03-2017	2	4
1	19-04-2017	2	5
1	19-03-2018	3	6
1	23-10-2019	2	7
2	24-09-2017	1	1
2	08-11-2017	2	2
2	10-09-2018	3	3
2	20-07-2020	3	4
3	10-11-2016	1	1
3	15-12-2016	2	2
3	20-12-2016	2	3
3	07-12-2017	2	4
3	18-12-2019	1	5
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/e30b243f-999d-4dfd-8ec9-10aaa208fb17)

12) rank all the transactions for each member whenever they are a zomato gold member for every non gold member transaction mark as na

userid	created_date	product_id	gold_signup_date	rnk	rnk
1	23-10-2019	2	43000	1	1
1	19-03-2018	3	43000	2	2
1	19-04-2017	2	NULL	0	na
1	11-03-2017	2	NULL	0	na
1	09-11-2016	1	NULL	0	na
1	20-05-2016	3	NULL	0	na
1	11-03-2016	1	NULL	0	na
2	20-07-2020	3	NULL	0	na
2	10-09-2018	3	NULL	0	na
2	08-11-2017	2	NULL	0	na
2	24-09-2017	1	NULL	0	na
3	18-12-2019	1	21-04-2017	1	1
3	07-12-2017	2	21-04-2017	2	2
3	20-12-2016	2	NULL	0	na
3	15-12-2016	2	NULL	0	na
3	10-11-2016	1	NULL	0	na
![image](https://github.com/TharunPrabu7/Zomato_analysis/assets/56309565/b571bb6d-32ea-48cb-9d0c-7b8c2ac2ad16)














