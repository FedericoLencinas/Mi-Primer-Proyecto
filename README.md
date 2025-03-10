# Mi-Primer-Proyecto
/*Cargar un vector de 5 números, sumarle a las posiciones pares 2 y a las impares 3 y
reemplazar los valores del vector. Finalmente mostrar todos los valores del vector
resultante.*/

int[] vec = new int[5];
for (int i = 0; i < vec.Length; i++)
{
    Console.WriteLine("ingrese un numero para la posicion "+i);
    vec[i] = int.Parse(Console.ReadLine());
    if (i%2== 0 )
    { vec[i] += 2; }
    else { vec[i] += 3; }
}
for (int i = 0; i < vec.Length; i++)
{
    Console.WriteLine($"Valor en la posición {i}: {vec[i]}");
}
Console.ReadKey();
