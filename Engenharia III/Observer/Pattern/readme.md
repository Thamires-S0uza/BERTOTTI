     package pattern;

     public abstract class Observer {
	   protected Subject subject;
	    public abstract void update();

<hr>

        Analógico.java
       
        package pattern;

        public class Analógico extends Observer {
      	public Analógico (Subject subject){
	      this.subject = subject;
	      this.subject.anexar(this);
     	}

	     @Override
	   public void update() {
		System.out.println("Analógico: " + Integer.toString(subject.getState()));		
    
    
 <hr>
 
    Digital.java
    
      package pattern;

        public class Digital extends Observer {
	      public Digital(Subject subject){
	      this.subject = subject;
	      this.subject.anexar(this);
	    }

	     @Override
	      public void update() {
		    System.out.println("Digital: " + Integer.toString(subject.getState() * 2));		
	     }    	
     }

<hr>

      

    
