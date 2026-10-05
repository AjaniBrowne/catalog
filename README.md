# Furniture Store Receipt Generator

## Description

This program simulates a furniture store checkout system. Product descriptions and prices are stored in variables, and a customer's purchases are added to a running total. The program then calculates sales tax and displays the customer's itemized order and final total.

## Products

### Lovely Loveseat

```python
lovely_loveseat_description = """
Lovely Loveseat. Tufted polyester blend on wood.
32 inches high x 40 inches wide x 30 inches deep.
Red or white.
"""
```

Price:

```python
lovely_loveseat_price = 254.00
```

### Stylish Settee

```python
stylish_settee_description = """
Stylish Settee. Faux leather on birch.
29.50 inches high x 54.75 inches wide x 28 inches deep.
Black.
"""
```

Price:

```python
stylish_sette_price = 180.50
```

### Luxurious Lamp

```python
luxurious_lamp_description = """
Luxurious Lamp. Glass and iron.
36 inches tall.
Brown with cream shade.
"""
```

Price:

```python
luxurious_lamp_price = 52.15
```

## Sales Tax

The store charges a sales tax of **8.8%**.

```python
sales_tax = 0.088
```

## Customer Purchase

Customer One purchases:

- Lovely Loveseat
- Luxurious Lamp

The program adds the prices of these items to the customer's total and stores the descriptions in an itemized list.

```python
customer_one_total += lovely_loveseat_price
customer_one_itemization += lovely_loveseat_description

customer_one_total += luxurious_lamp_price
customer_one_itemization += luxurious_lamp_description
```

## Tax Calculation

The sales tax is calculated and added to the subtotal.

```python
customer_one_tax = customer_one_total * sales_tax
customer_one_total += customer_one_tax
```

### Calculation

```text
Subtotal:
254.00 + 52.15 = 306.15

Tax:
306.15 × 0.088 = 26.9412

Final Total:
306.15 + 26.9412 = 333.0912
```

## Sample Output

```text
Customer One Items:

Lovely Loveseat. Tufted polyester blend on wood.
32 inches high x 40 inches wide x 30 inches deep.
Red or white.

Luxurious Lamp. Glass and iron.
36 inches tall.
Brown with cream shade.

Customer One Total:
333.0912
```

## How It Works

1. Product descriptions and prices are stored in variables.
2. The customer's purchased items are added to an itemized list.
3. Product prices are added to a running subtotal.
4. Sales tax is calculated at 8.8%.
5. The tax is added to the subtotal to produce the final total.
6. The program prints the itemized receipt and total purchase amount.
