def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        return price - (price * (discount_percent / 100))
    return price

while True:
    price = float(input("Enter the original price: "))
    discount_percent = float(input("Enter the discount percentage: "))

    final_price = calculate_discount(price, discount_percent)

    if final_price == price:
        print(f"No discount applied. Final price: Ks{final_price: }")
    else:
        print(f"Discount applied! Final price: Ks{final_price: }")
