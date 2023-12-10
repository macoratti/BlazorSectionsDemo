Blazor Sections são usadas para controlar o conteúdo em um componente  pai a partir do componente filho

Para isso usamos dois componentes integrados  :

**SectionOutlet**: Renderiza o conteúdo fornecido pelos componentes SectionContent com argumentos 
SectionName ou SectionId correspondentes. 
_(Dois ou mais componentes SectionOutlet não podem ter o mesmo SectionName ou SectionId.)_

**SectionContent**: Fornece conteúdo como um RenderFragment para componentes SectionOutlet com um 
SectionName ou SectionId correspondente. 
(_Se vários componentes SectionContent tiverem o mesmo SectionName ou SectionId, o componente 
SectionOutlet correspondente renderizará o conteúdo do último SectionContent renderizado_.)

As seções podem ser usadas em layouts e em componentes pai-filho aninhados.

Para criar uma seção usamos um objeto SectionOutlet identificado por um **SectionName** ou pelo parâmetro SectionId.

O parâmetro SectionName é uma string usada para direcionar o SectionOutlet de um componente SectionContent.
O argumento passado para SectionName geralmente o formato kebab case  (Ex: top-section , nome-arquivo, nav-bar )

Se houver mais de uma seção definida elas devem ter SectionName ou SectionId diferentes

Assim O que torna as seções possíveis no Blazor são os objetos S**ectionOutlet e SectionContent** que estão presentes no namespace

**@using Microsoft.AspNetCore.Components.Sections**

que podemos definir no arquivo _Imports.razor 
  
