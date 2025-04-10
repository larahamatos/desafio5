# desafio5

#  questao1
        int contadorN, numero, contadorPar, contadorImpar, nulos;
        Scanner ler = new Scanner(System.in);
        
        contadorN = 1;
        contadorPar = 0;
        contadorImpar = 0;
        nulos = 0;
        
        while (contadorN <= 30) {
            System.out.println("Digite um numero:");
            numero = ler.nextInt();
            if (numero == 0) {
                nulos++;
            } else if(numero % 2 == 0){
                contadorPar++;
            } else {
                contadorImpar++;
            }
            contadorN++;
        }
        System.out.println("Quantidade de nulos: "+nulos);
        System.out.println("Quantidade de pares: "+contadorPar);
        System.out.println("Quantidade de impares: "+contadorImpar);

# questao2
        int numero;
        
        numero = 1000;
        
        while ( numero <= 1999 ) {
            if ( numero % 11 == 5) {
                System.out.println(numero);
            }
            numero++;
            
# questao3
        int c, n, cd, cf;
        Scanner ler = new Scanner(System.in);

        c = 1;
        cd = 0;
        cf = 0;

        while (c <= 10) {
            System.out.println("Informe um número: ");
            n = ler.nextInt();
            if (n >= 10 && n <= 20) {
                cd++;
            } else {
                cf++;
            }
            c++;
        }
        System.out.println("Entre 10 e 20 tem: "+cd);
        System.out.println("Fora do intervalo tem: "+cf);

# questao4
int chico, ze, anos;
        
        chico = 150;
        ze = 110;
        anos = 0;
        
        while ( chico > = ze ) {
            chico = chico + 2;
            ze = ze + 3;
            anos++; 
            System.out.println("Zé: "+ze+" Chico: "+chico);
        }
        System.out.println("Zé levou "+anos+" anos para ser maior que Chico!");

# questao5
        int numero, cont025, cont2650, cont5175, cont76100;
        Scanner ler = new Scanner (System.in);
        
        cont025 = 0;
        cont2650 = 0;
        cont5175 = 0;
        cont76100 = 0;
        numero = 0;
        
        while ( numero >= 0) {
            System.out.println("Digite um número: ");
            numero = ler.nextInt();
            if ( numero >= 0 && numero <= 25) {
                cont025++;
            } else if ( numero >= 26 && numero <= 50 ) {
                cont2650++;
            } else if ( numero >= 51 && numero <= 75) {
                cont5175++;
            } else if ( numero >= 76 && numero <= 100) {
                cont76100++;
            } else {
                System.out.println("Intervalo não contabilizado apenas de 0 a 100");
            }
            System.out.println("[0,25]: "+cont025+" [26,50]: "+cont2650+" [51,75]: "+cont5175+" [76,100]: "+cont76100);
