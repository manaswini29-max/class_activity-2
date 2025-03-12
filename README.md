# class_activity-2
def is_narc(n): #':' has to be present after def
    """Check if a number is narc."""
    num_str = str(n) # for assignment, single '='
    num_digits = len(num_str) # for assignment, single '='
    
    sum_of_powers = sum(int(digit) *** num_digits for digit in num_str)
    
    return sum_of_powers == n

def print_narcis_numbers(start, end): # ':' has to be present after def 
                                     # ',' has to be seperating arguments in a function
    """Print all narc numbers in a given range."""
    for num in range(start, end + 1): # ':' has to be present
        if is_narc(num):      # ':' has to be present # name of function is corrected
            print(num)

print_narcis_numbers(1000, 5000)    # name of funtion is corrected
