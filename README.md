# box-turtle
### web wallet in a box - Dont expose this to the internet or you'll lose everything. 

Start up walletd:

`./walletd --wallet-file YOURWALLET.wallet --password YOURPASSWORD --rpc-password test --daemon-address public.turtlenode.io`

Alternatively, you can remove the --daemon-address arg to use a local TurtleCoind you've got open.

If you want to change the RPC password, set it in the config.js file.

Currently CORS will prevent this from just werking, so for now you can launch chromium like this to test it out until CORS is fixed:

`chromium index.html --disable-web-security --user-data-dir .`

- [ ] TODO: Add last 10 transactions
- [ ] TODO: Add output window so the user knows where to expect to look for output
- [ ] TODO: Add CORS header to walletd
- [ ] TODO: Payment ID's
- [ ] TODO: Get users address
