@[user]:
Fix the Day.js bug in repo/.

Problem: Formatting years below 1000 with YYYY omits leading zeroes,
producing values such as 1 instead of 0001.

Expected fix: Pad the YYYY formatter output to four digits for years
below 1000.

Validate with:
npx jest test/display.test.js --runInBand --coverage=false