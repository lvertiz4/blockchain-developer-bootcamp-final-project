i.	SWC-103 (Floating pragma)
  1.	Specific compiler pragma 0.8.0 used in contracts to avoid accidental bug inclusion through outdated compiler versions.

ii.	Modifiers used only for validation
  1.	OnlyOwner modifier from Ownable.sol validates data with require statements.

iii.	Pull over push
  1.	All functions that modify state are based on receiving calls rather than making contract calls.

