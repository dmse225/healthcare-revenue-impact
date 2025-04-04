def calculate_revenue_impact(base_fees, visit_volumes, incentive_percent): 
    """
    Calculates the total revenue impact of an incentive adjustment.
    
    Parameters:
    base_fees (list): List of base fee schedules for each CPT code.
    visit_volumes (list): Corresponding visit volumes for each CPT code.
    incentive_percent (float): Outcome Incentive percentage (e.g., 10 for 10%).
    
    Returns:
    float: Total additional revenue from the incentive adjustment.
    """
    total_impact = sum((fee * volume * (incentive_percent / 100)) for fee, volume in zip(base_fees, visit_volumes))
    return total_impact

# Example Usage
base_fees = [50, 75, 100] # Example CPT code fees
visit_volumes = [1500, 2000, 1000] # Example visit volumes
incentive_percent = 10 # Example incentive percentage

total_revenue_impact = calculate_revenue_impact(base_fees, visit_volumes, incentive_percent)
print(f"Total Revenue Impact: ${total_revenue_impact:,.2f}")
