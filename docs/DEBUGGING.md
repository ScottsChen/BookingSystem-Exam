# Debugging – Booking System

## Bug 1
**Problem:**
Datum och tid för bokningarna är osorterade.
**Cause:**
BookingService GetActiveBookings saknar filtreringsinnehåll
**Solution:**
Lägger till Filtrering, Aktiva bokningar syns, Bokingarna visas först i datums ordning och sedan StartTids ordning.
**Testing:**
Testkörning visar att aktiva bokningar visas i ordningen datum, starttid.
## Bug 2
**Problem:**
Hittar inte Bokning om man inte stavar Exakt
**Cause:**
Metoden saknar Contains(name,StringComparison.OrdinalIgnoreCase), Denna kod löser det problemmet.
**Solution:**
har nu lagt till hjälp medel i metoden så att programmet hittar namnet vid använding av små eller stora bokstäver samt matchande bokstäver och att bokningen måste vara aktiv för att kunna visas med hjälp av &&.
**Testing:
case 2 kan nu känna igen bokningar som delar samma bokstav och små bokstäver.


## Bug 3
**Problem:**
Avbokning gick inte att utföra
**Cause:**
BookingService, BookingResult Cancel
**Solution:**

**Testing: