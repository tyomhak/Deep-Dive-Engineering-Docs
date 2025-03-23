[Solution Link](https://github.com/tyomhak/EngineeringDeepDive/blob/main/Cpp/03/practice.cpp)

1) multi_array template-ի մեջ ավելացնել "static constexpr int volume = ..." դաշտ, որը ցույց կտա ընդհանուր վանդակների քանակը այդ կառուցվածքում։
2) Իրականացնել multi_array_accessor template, որի պարամետրերը կլինեն հենց ինքը multi_array-ը ու ինդեքսների variadic հաջորդականությունը։ Նպատակն է՝ հասանելիություն ստանալ կոնկրետ վանդակներին։
3) tuple դասի getter-ը ձևափոխել այնպես, որ ինդեքսով overflow-ի ժամանակ մենք compile error տեսնենք։ Հիշենք որ tuple-ի ինդեքսները compile time հայտնի մեծություններ են։
4) Իրականացնել երկու tuple-ների համեմատման օպերատոր "operator==":

