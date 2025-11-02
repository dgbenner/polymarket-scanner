# Sample Data Structure

## What We're Tracking

Based on Polymarket large bet data, each entry contains:

### Market Information
- **Market Question**: The prediction being bet on
  - Example: "Will Zohran Mamdani win the 2025 NYC mayoral election?"
  - Example: "Mariners vs. Blue Jays"
  - Example: "Will Catherine Connolly win the Irish Presidential Election?"

- **Wallet Address**: The trader's blockchain address
  - Format: Long hexadecimal string (e.g., `0xebdbfcf7b4401addc8b4031770a1ab942bb105413bed453d54f9425cd9f211a9`)

### Bet Details
- **Outcome**: What the trader is betting on
  - Examples: "Yes", "No", "Blue Jays", "Jets"

- **Side**: Direction of the bet
  - `BUY` (green badge) - Betting that outcome will happen
  - `SELL` (red badge) - Betting that outcome won't happen

- **Price**: The odds/probability
  - Range: 0.01 to 1.00
  - Example: 0.933 = 93.3% implied probability
  - Example: 0.54 = 54% implied probability

- **Size**: Amount of the bet
  - Displayed in dollars
  - Examples: $1,860, $2,500, $2,770, $11,550

## Market Categories We Track

Based on observed data:

### Politics
- NYC mayoral election predictions
- Irish Presidential Election predictions
- US federal elections

### Sports
- MLB games (Mariners vs. Blue Jays)
- NHL games (Jets vs. Flames)
- Soccer matches (West Ham vs. Brentford)

### Notable Patterns

**Whale Activity Indicators:**
- Bets over $10,000
- Multiple large bets from same wallet
- High probability bets with large size (e.g., 0.999 price with $1,114 size)

**Market Intelligence:**
- When whales buy high probability outcomes (0.9+), they're very confident
- SELL positions on high probability markets indicate contrarian betting
- Large bets on sporting events often placed close to game time

## Use Cases

As mentioned in analysis:

1. **Tracking whale activity** - Monitoring when large bettors place significant bets on prediction markets

2. **Market intelligence** - Using these large bets as signals about what informed traders believe will happen

3. **Finding opportunities** - Spotting where big money is moving, which could indicate insider knowledge or strong convictions about outcomes

## Data Points to Display

Minimum viable display:
- Market question
- Outcome being bet on
- BUY or SELL indicator
- Price (probability)
- Bet size

Enhanced display (future):
- Wallet address (for tracking repeat whales)
- Timestamp of bet
- Market category
- Total volume on market
- Price movement after bet placed
