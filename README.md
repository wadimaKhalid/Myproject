//A simple Java program that simulates a voting process. Users can vote for their preferred candidate, and the program counts the votes and announces the winner.
import java.util.Scanner ;
public class Voting {
  public static void main (String [] args ) {
    int langu , age ,gender ,Vote=0 ;
     int Wadima=0 , Retaj=0 ,Reem=0 , Maram=0 , Fatima=0 ;
    Scanner input = new Scanner (System.in) ;
     
     for (int a=0 ;a<10;a++) {
    System.out.println ( " choose language 1.English , 2.Arabic ") ;
    langu = input.nextInt() ;
    if ( langu ==1 ) {
       System.out.println ( "Enter your age ") ;
   age = input.nextInt() ;
   if ( age<=21 )
     System.out.println ( "Thank you") ;
     else  {
     System.out.println ( "1.male , 2.Female") ;
     gender = input.nextInt() ;
      System.out.println ( " 1.Wadima 2.REtaj 3.Reem 4.Maram 5.Fatima") ;
        Vote = input.nextInt() ;
        System.out.println ( "Thank you") ; }
      }
   
    else {
 
       System.out.println ( "ادخل عمرك") ;
   age = input.nextInt() ;
   if ( age<=21 )
     System.out.println ( " شكرا لك") ;
     else  {
     System.out.println ( "1.ذكر 2.انثى ") ;
     gender = input.nextInt() ;
      System.out.println ( " 1.وديمه 2.رتاج 3.ريم 4.مرام 5.فاطمة") ;
        Vote = input.nextInt() ;
      System.out.println ( "شكرا لك") ;
     }
      }
 if (Vote==1) Wadima++ ;
    else if (Vote==2) Retaj++ ;
    else if (Vote==3) Reem++ ;
    else if (Vote==4) Maram++ ;
    else if ( Vote==5) Fatima++ ;
    }
   
 System.out.println( "Voting Summary" );
        System.out.println ( "Wadima :" +Wadima ) ;
         System.out.println( "Retaj :" +Retaj ) ;
          System.out.println( "Reem :" +Reem ) ;
           System.out.println( "Maram :" +Maram ) ;
         System.out.println ( "Fatima :" +Fatima ) ;
         
         int max = Wadima ;
         String winner = " Wadima " ;
         if ( Retaj > max ) {
           max = Retaj ;
           winner = " Retaj " ; }
          if ( Reem > max ) {
           max = Reem ;
           winner = " Reem " ; }
           if ( Maram > max ) {
           max = Maram ;
           winner = " Maram" ; }
            if ( Fatima> max ) {
           max = Fatima ;
           winner = " Fatima" ; }
             System.out.println ( " the winner is : " +winner ) ;
       
  }
}
