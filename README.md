                case 2 -> {System.out.println("Usted ha seleccionado Triangulos y mas Triangulos");
                        int subopc=0;
                        System.out.println("submenu");
                        System.out.println("1) Quiero dibujar un triangulo rectangulo: ");
                        System.out.println("2) Quiero dibujar un triangulo Equilatero");
                        subopc = entry.nextInt();
                      if (subopc == 1) {
                          System.out.println("Ingrese la altura que desea: ");
                          int alt = 0;
                          alt = entry.nextInt();
                          for (int i = 1; i <= alt; i++) {
                              for (int j = 1; j <= alt - i; j++) {
                                  
                                  System.out.print(" ");
                              }
                              for (int k = 1; k <= (2 * i - 1); k++) {
                            
                                  System.out.print("*");
                              }                              
                              System.out.println();
                          }
                    } else if (subopc == 2){
                          System.out.println("Ingrese la altura que desea: ");
                          int altura=0;
                          altura = entry.nextInt();
                          for (int i = 0; i < altura; i++) {
                              for (int j = 0; j < i; j++) {
                                  System.out.print("*");
                              }
                              System.out.println();
                          }
                    }
                }
                case 3 -> {System.out.println("");
                    System.out.println("Palabras palindromas");
                    System.out.println("Anita lava la tina");
                    System.out.println("Ingrese la palabra palindroma");
                    String cadena = entry.next();//donde se ingresa
                    String cadena1= ""; //sirve como acumulador
                    for (int i = cadena.length()-1; i >= 0; i--) {
                        cadena1+=cadena.charAt(i); //mueve las posiciones
                    }
                    String pal = cadena1.toLowerCase();
                    if (cadena.equals(cadena1)) {
                        System.out.println("La palabra "+pal+" es palindroma");
                    }else 
                        System.out.println("La palabra "+pal+" no es palindroma");
                }
