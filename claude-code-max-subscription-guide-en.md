# Claude Code Max Subscription Usage Guide

## Overview

Claude Code is Anthropic's official CLI tool, providing developers with powerful AI-assisted programming capabilities. This document details the usage rules and limitations for Claude Code Max subscription plans.

## Subscription Plan Comparison

### Plan Types and Pricing

| Plan Name | Monthly Fee | Target Users |
|-----------|-------------|--------------|
| Pro | $20 | Standard users |
| Max 5x Pro | $100 | Professional users |
| Max 20x Pro | $200 | Heavy users |

## Dual Rate Limit System

Claude Code employs a dual rate limit mechanism to ensure service stability and fair usage:

### 1. 5-Hour Reset Limits (Existing)

Usage quotas that reset every 5 hours:

- **Pro Plan**
  - Approximately 10-40 Claude Code prompts

- **Max 5x Pro Plan**
  - Approximately 50-200 Claude Code prompts
  - Approximately 225 Claude messages

- **Max 20x Pro Plan**
  - Approximately 200-800 Claude Code prompts
  - Approximately 900 Claude messages

### 2. Weekly Reset Limits (New)

New limits effective from August 28, 2025, resetting every 7 days:

#### Pro Plan ($20/month)
- 40-80 hours of Sonnet 4 usage per week

#### Max 5x Pro Plan ($100/month)
- 140-280 hours of Sonnet 4 usage per week
- 15-35 hours of Opus 4 usage per week

#### Max 20x Pro Plan ($200/month)
- 240-480 hours of Sonnet 4 usage per week
- 24-40 hours of Opus 4 usage per week

## Automatic Model Switching

Claude Code automatically switches from premium to standard models when specific usage thresholds are reached:

- **Max 5x Pro**: Automatically switches from Opus 4 to Sonnet 4 at 20% of rate limit
- **Max 20x Pro**: Automatically switches from Opus 4 to Sonnet 4 at 50% of rate limit

## Useful Commands

- `/status` - Check remaining usage quota
- `/model` - Manually select model at the beginning of a session

## Key Takeaways

1. **Dual Limits Apply Simultaneously**: Users must comply with both 5-hour and weekly limits
2. **Automatic Reset**: Limits reset automatically without manual intervention
3. **Limited Impact**: New weekly limits are expected to affect less than 5% of users (mainly those running 24/7)
4. **Overage Purchase Option**: Max subscribers can purchase additional usage at standard API rates after reaching limits
5. **Usage Variability**: Actual usage may vary based on codebase size and other factors

## Why Introduce Weekly Limits?

Main reasons for Anthropic's introduction of weekly limits:
- Address "unprecedented demand" since launch
- Prevent a small minority of users from running Claude Code continuously 24/7 in the background
- Ensure reliable, stable service for all users
- Balance resource allocation and improve overall user experience

## Frequently Asked Questions

### Q: When do weekly limits reset?
A: Automatically every 7 days, calculated from first use.

### Q: What happens if I reach both 5-hour and weekly limits?
A: Reaching either limit triggers usage restrictions; you'll need to wait for the respective reset time.

### Q: Will most users be affected?
A: No. According to Anthropic's statistics, over 95% of users won't be affected by the new limits.

## Changelog

- July 28, 2025: Anthropic announces new weekly limit plan
- August 28, 2025: Weekly limits take effect

## Resources

- [Anthropic Official Help Center](https://support.anthropic.com/)
- [Claude Code Official Documentation](https://docs.anthropic.com/en/docs/claude-code)