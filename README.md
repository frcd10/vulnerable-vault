# vault

A minimal Anchor program: one SOL vault per owner. Anyone can deposit; the owner withdraws.

- `initialize` creates the vault PDA (`["vault", owner]`) and stores the owner.
- `deposit(amount)` transfers lamports from the depositor into the vault.
- `withdraw(amount)` moves lamports from the vault to the owner's wallet.

Not audited. Do not deploy with real funds.
