# Stacks Timelock

Time-locked transactions and vesting on Stacks.

## Features
- Schedule future payments
- Token vesting schedules
- Cancellable by creator
- Extendable lock periods

## Use Cases
- Employee vesting
- Scheduled payments
- Escrow with time component
- Trust funds

## Functions
```clarity
(create-timelock (beneficiary) (amount) (unlock-delay) (memo))
(execute-timelock (lock-id))
(cancel-timelock (lock-id))
(extend-timelock (lock-id) (additional-blocks))
(is-unlocked (lock-id))
(get-time-remaining (lock-id))
```

## License
MIT

