### Documentação
* `Class<T>`
  * `newInstance()` da classe `Class<T>` foi descontinuado a partir do JDK 9, pois não verificava Exceptions checked.
  * `Constructor<T>`
    * `setAccessible(boolean flag)` informar para classe que é para tornar os métodos privados em públicos.
    * `newInstance()` da classe `Constructor<T>` válida Exceptions checked.
    * `getConstructor()` recupara construtor **público** com ou sem parâmetro.
    * `getConstructors()` recuperar todos construtores publicos.
    * `getDeclaredConstructor()` recupara construtor **público** ou **privado** com ou sem parâmetro.
    * `getDeclaredConstructors()` recupera todos construtores públicos e privados.
  * `getMethod(String nomeDoMetodo, Class<?> ...tiposArgs)` recupera método **públicos** com ou sem parâmetros incluindo o método da classe pai.
  * `getMethods()` recupera todos os métodos **públicos** com ou sem parâmetros incluindo os métodos da classe pai.
  * `getDeclaredMethod(String nomeDoMetodo, Class<?> ...tiposArgs)` recupera método **públicos** ou **privados** com ou sem parâmetros, apenas para o método da própria classe.
  * `getDeclaredMethods()` recupera todos os métodos **públicos** ou **privados** com ou sem parâmetros, apenas para os métodos da própria classe.
   * `Method<T>` é retornado em cada um dos métodos a cima.
     * `invoke(Object obj, Object... args)` invoca o método do objeto que desejar, o primeiro parâmetro representa a instância do objeto que se quer executar, o segundo parâmetro é um varargs com todos os parâmetros que o método precisa receber. caso o método chamado seja `void` o retorno é `null`;
  
  
 
