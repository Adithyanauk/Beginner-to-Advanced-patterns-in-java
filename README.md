                                                    # Beginner-to-Advanced-patterns-in-java

class solidrectangle{
    void print(){
    for(int i=0;i<4;i++){
        for (int j = 0; j < 5; j++) {
        System.out.print("*");
        }
        System.out.println(" ");
    }
}
}

class hollowrectangle{
    void output(){
        int n=4;
        int m=5;
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= m; j++) {
                if(i==1 || j==1 || i == n || j==m ) {
                    System.out.print("*");
                }
                else{
                    System.out.print(" ");
                }
            }
            System.out.println(); 
        }
    }
}

class halfpyramid{
    void print(){
    int n=4;
    for(int i=1;i<=n;i++){
        for(int j=1;j<=i;j++){
        System.out.print("*");
        }
        System.out.println();
    }
}
}

class invertedhalfpyramid{
    void print(){
        int n=4;
        for (int i=1;i<=n;i++) {
            for (int j=1; j <=(n-i); j++) {
                System.out.print(" ");                
            }
            for (int j = 1; j <=i; j++) {
                System.out.print("*");
            }
            System.out.println();

            
        }
    }
}

class halfnumberpyramid{
    void print(){
        int n =5;
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print(j+" ");
            }
            System.out.println( );
        }
    }
}

class InvertedNumberHalfPyramid{
    void print(){
        int n=5;
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j<=n-i+1; j++) {
                System.out.print(j+" ");
            }
            System.out.println( );
        }
    }
}

class floidstriangle{
    void print(){
        int n =5;
        int number =0;
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= i; j++) {
                number++;
                System.out.print(number+" ");
            }
            System.out.println( );
        }
    }
}

class binaryTriangle{
    void print(){
        int n =5;
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= i; j++) {
                int sum =i+j;
                if(sum%2 == 0){
                    System.out.print("1"+" ");
                }else{
                    System.out.print("0"+" ");
                }
            }
            System.out.println( );
        }
    }
}

class Solidrhombus{
    void print(){
    int n=5;
    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= n-i; j++) {
            System.out.print(" ");
        }
        for (int j = 1; j <= n; j++) {
            System.out.print("* ");
        }
        System.out.println();
    }
    }
}

class NumberPyramid{
    void print(){
        int n=5;
        int number = 0;
        for (int i = 1; i <= n; i++) {
            number++;
            for (int j = 1; j <= n-i; j++) {
                System.out.print(" ");
            }
            for (int j = 1; j <= i; j++) {
                System.out.print(number+" ");
            }
            System.out.println();
        }
        } 
}

class palindromeNumberPyramid{
    void print(){
        int n=5;
        int number = 0;
        for (int i = 1; i <= n; i++) {
            number++;
            for (int j = 1; j <= n-i; j++) {
                System.out.print(" ");
            }
            for (int j = i; j >= 1; j--) {
                System.out.print(j);
            }
            for (int j = 2; j <= i ; j++) {
                System.out.print(j);
            }
            System.out.println();
        }
        } 
}

class butterflypattern{
    void print(){
        int n=4;
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <=i; j++) {
                System.out.print("* ");    
            }
            int space =2*(n-i);
            for (int j = 1; j <=space; j++) {
                System.out.print("  ");
            }
            for (int j = 1; j <=i; j++) {
                System.out.print("* ");    
            }
            System.out.println();

            
        }
        for (int i = n; i >=1; i--) {
            for (int j = i; j >=1; j--) {
                System.out.print("* ");    
            }
            int space =2*(n-i);
            for (int j = 1; j <=space; j++) {
                System.out.print("  ");
            }
            for (int j = i; j>=1; j--) {
                System.out.print("* ");    
            }
            System.out.println();

            
        }
       }
}

class diamondpattern{
    void  print(){
        int n=4;
        for(int i=1;i<=n;i++){
            //space
            for (int j = 1; j <=n-i; j++) {
                System.out.print("  ");
            }
            for (int j = 1; j <=i; j++) {
                System.out.print("* ");
            }
            for (int j = 2; j <=i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
        for(int i=n;i>=1;i--){
            //space
            for (int j = 1; j <=n-i; j++) {
                System.out.print("  ");
            }
            for (int j = i; j >=1 ; j--) {
                System.out.print("* ");
            }
            for (int j = i; j >=2; j--) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}

class hollowbutterfly{
    void print(){
        int n=5 ;
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= i; j++) {
                if ( j==1  || j==i){
                    System.out.print("*");
                }else{
                    System.out.print(" ");
                }
            }
            int space =2*(n-i);
            for (int j = 1; j <= space; j++) {
                System.out.print(" ");
            }
            for (int j = 1; j <= i; j++) {
                if ( j==1  || j== i){
                    System.out.print("*");
                }else{
                    System.out.print(" ");
                }
            }
            System.out.println();
        }

        for (int i = n; i >= 1; i--) {
            for (int j = 1; j <= i; j++) {
                if ( j==1  || j==i){
                    System.out.print("*");
                }else{
                    System.out.print(" ");
                }
            }
            int space =2*(n-i);
            for (int j = 1; j <= space; j++) {
                System.out.print(" ");
            }
            for (int j = 1; j <= i; j++) {
                if ( j==1  || j== i){
                    System.out.print("*");
                }else{
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
}

class Solidhollowrhombus{
    void print(){
    int n=5;
    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= n-i; j++) {
            System.out.print(" ");
        }
        for (int j = 1; j <= n; j++) {
            if(j==1 || j==n ||i==1||i==n){
            System.out.print("*");
            }else{
                System.out.print(" ");
            }
        }
        System.out.println();
    }
    }
}

class pascalstriangle{
    void print(){
        int n=5;
        for (int i = 1; i <=n; i++) {
            for (int j = 1; j <= n-i; j++) {
              System.out.print(" ");  
            }
            int coef =1;
            for(int j=1;j<=i;j++){
                System.out.print(coef+ " ");
                coef = coef * (i - j) / j;
            }
            System.out.println();
            
        }
    }
    
}

public class patterns {
    public static void main(String[] args) {
        //solid rectangle
       solidrectangle sr=new solidrectangle();
       sr.print();
       System.out.println("\n");
        //hollow rectangle
        hollowrectangle hr=new hollowrectangle();
        hr.output();
        System.out.println("\n");
        //half pyramid
        halfpyramid hp=new halfpyramid();
        hp.print();
        System.out.println("\n");
        //inverted half pyramid
        invertedhalfpyramid hlp =new invertedhalfpyramid();
        hlp.print();
        System.out.println("\n");
        //half number pyramid
        halfnumberpyramid hnp = new halfnumberpyramid();
        hnp.print();
        System.out.println("\n");
        //InvertedNumberHalfPyramid
        InvertedNumberHalfPyramid inhp = new InvertedNumberHalfPyramid();
        inhp.print();
        System.out.println("\n");
        //floid's triangle
        floidstriangle ft =new floidstriangle();
        ft.print();
        System.out.println("\n"); 
        //binary triangle
        binaryTriangle bt =new binaryTriangle();
        bt.print();
        System.out.println("\n");  
        //solid rectangle
        Solidrhombus srb =new Solidrhombus();
        srb.print();
        System.out.println("\n");
        //number triangle 
        NumberPyramid np = new NumberPyramid();
        np.print();
        System.out.println("\n");
        //palindrome number pyramid 
        palindromeNumberPyramid pnp = new palindromeNumberPyramid();
        pnp.print();
        System.out.println("\n");
        //butterfly pattern
        butterflypattern bp=new butterflypattern();
        bp.print();
        System.out.println("\n");
        //diamond pattern
        diamondpattern dip = new diamondpattern();
        dip.print();
        System.out.println("\n");
        //hollow butterfly
        hollowbutterfly hb =new hollowbutterfly();
        hb.print();
        System.out.println("\n");
        //solid hollow rombus
        Solidhollowrhombus shb = new Solidhollowrhombus();
        shb.print();
        System.out.println("\n");
        //pascals triangle
        pascalstriangle pt =new pascalstriangle();
        pt.print();
        System.out.println("\n");
    }
}
