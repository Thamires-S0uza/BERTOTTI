pagamento.java;

package pattern;

public class Pagamento {

     private Pagar pagar ;

     public void setPagar ( Pagar pagar ) {
                    this.pagar = pagar;

      }
      
     public void pagarConta () {
                    this.pagar.pagarConta();
      }


}

      ----------------------------------------------------------------

  pagarDebito.java
  
  package pattern

      public interface Pagar {

         public void pagarConta();

     } 
     --------------------------------------------------------------------
     
     package pattern;

public class pagarDebito implements Pagar{

        public void pagarConta() {
             System.out.println("Pagou conta no débito.");
        }


----------------------------------------------------------------------------
pagarCredito.java

    package pattern;

        public class pagarCredito implements Pagar {

          public void pagarConta() {
                  System.out.pintln("Pagou conta no crédito.");

      }

} 


}

----------------------------------------------------------------------

pagarPayPal.java

    package pattern;

    public class pagarPayPal implements Pagar {

      public void pagarConta() {

        System.out.println("Pagou conta no PayPal.");

     }

}

