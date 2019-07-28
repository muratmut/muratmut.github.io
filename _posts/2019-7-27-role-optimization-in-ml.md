---
layout: post
title: The role of Optimization in Statistics and Machine Learning
---

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin vitae neque quis ante convallis accumsan. Duis id ultrices eros. Interdum et malesuada fames ac ante ipsum primis in faucibus. In hac habitasse platea dictumst. Donec euismod ultricies massa eu cursus. Vestibulum in ultricies metus. Sed egestas nisl eget elit sollicitudin venenatis. Sed faucibus felis a felis dictum, a malesuada sapien facilisis. Etiam massa nisi, malesuada ac quam nec, sollicitudin porta ipsum. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.

#####```python
def main():
    # change the path below to the folder having .csv data
    path = '/cg1/SF_estimation_testcases/NielsenMix/QPData/new_contract_data/qp10/'

    controller_table = controller_file_from_csv(path)
    variable_desc = get_categorical_vars(path)

    raw_data_df, hc = raw_data_spark_df(path, variable_desc)

    interactions = [Interaction('var1', []),
                    Interaction('var2', [])
                    ]

    qp_solver_input = QPSolverInput(controller_pd=controller_table, raw_data=raw_data_df, interactions=interactions, csv_path=path, spark=hc, debug=True)


    controller = QPSolverControl(qp_solver_input)

    qp_status, solution = controller.run()
    print qp_status

```

Integer aliquet tincidunt ante, nec dapibus ex dapibus in. Curabitur vestibulum congue ex et maximus. Proin suscipit auctor risus vitae dapibus. Maecenas eu nisl ante. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Etiam lacus arcu, hendrerit id porttitor vitae, bibendum ut massa. In consequat, neque sit amet tristique fermentum, orci urna rhoncus tellus, et molestie sapien ligula nec nisl. Aenean condimentum condimentum magna ut pellentesque. Donec maximus mi non velit scelerisque, ac placerat arcu porta.

Fusce sed libero eget elit faucibus vulputate. Duis blandit laoreet neque, in tempus elit facilisis vitae. Etiam magna mi, iaculis vel urna eget, pellentesque tincidunt lacus. Fusce sapien arcu, commodo in justo in, posuere maximus urna. Proin rhoncus quis orci sed lacinia. Quisque suscipit felis nec pharetra iaculis. Nunc lobortis, velit vel luctus vehicula, magna urna efficitur nibh, vel finibus ligula lorem in nulla. Proin id nibh quam. Nullam fringilla, velit luctus luctus tincidunt, sapien velit vehicula leo, at semper diam turpis vel nisl. Nam venenatis ac urna sit amet porttitor. Nullam luctus orci erat, ultrices tincidunt quam laoreet at. Aliquam erat volutpat. Pellentesque dapibus diam at massa ullamcorper, cursus tempus tellus porttitor.

Pellentesque tincidunt, neque at tempor dapibus, eros neque dapibus tortor, sit amet molestie libero turpis non leo. Vestibulum vel accumsan justo. Vivamus lacinia euismod lacus a varius. Duis pellentesque ex sapien, non semper ipsum sollicitudin id. Integer a enim odio. Nullam molestie quam velit, vel varius arcu venenatis a. In in erat vitae eros pellentesque aliquet. Praesent suscipit tincidunt dignissim. Donec interdum magna a tristique sodales. Cras luctus urna mauris, vel commodo justo interdum vel. Phasellus ultricies pretium libero. Maecenas elementum, lectus in posuere fermentum, velit ligula consectetur erat, vel consectetur risus sem ut sem.

Duis tempus rhoncus erat, in aliquet nulla aliquam a. Duis varius accumsan purus at egestas. Integer iaculis velit vitae neque rhoncus commodo. Proin nec lectus faucibus massa volutpat gravida. Vestibulum velit leo, condimentum at lectus et, congue tincidunt ex. Donec aliquam, dui eget semper feugiat, massa turpis pretium massa, quis interdum orci augue in erat. Nullam sit amet eros pellentesque, iaculis nisi id, tincidunt velit. In ornare purus tortor, pulvinar sagittis nibh blandit non. Nam dictum nisi est, eget ornare elit facilisis at. Suspendisse potenti. Nunc id nibh eu lacus rutrum cursus. Nullam mi nisl, maximus egestas varius sed, pretium ut risus. Nulla sapien metus, blandit in ante quis, auctor semper nibh. Quisque nec luctus urna. Vivamus convallis odio at scelerisque lacinia.

Etiam ut maximus orci, sed vulputate tortor. Pellentesque ut faucibus enim. Curabitur blandit dui in sem vestibulum dictum. Vestibulum in suscipit justo. Maecenas gravida augue enim, ut dignissim diam pulvinar vitae. Phasellus finibus enim consequat metus rhoncus suscipit. Cras sed ligula enim. Proin id luctus eros. Vestibulum erat leo, sodales eleifend pharetra et, tristique eu ex. Sed ac sem pharetra, vehicula eros at, fringilla mauris. In vestibulum efficitur fermentum. Vestibulum sollicitudin ultricies tellus, ac semper nunc aliquam non.

Integer ac dolor condimentum, pretium purus in, placerat magna. Phasellus tristique bibendum quam laoreet tristique. Aenean sed libero sit amet nibh sagittis tempor. Aliquam efficitur enim eget condimentum tempor. Pellentesque tempor neque sed consectetur rutrum. Proin eu enim felis. Nullam consectetur sed nibh at pellentesque. Integer hendrerit risus ac turpis lobortis, at sodales magna vulputate. Maecenas aliquet rhoncus blandit. Nunc vitae suscipit diam. Cras gravida sodales ante, sit amet tincidunt eros semper vel.

Aliquam erat volutpat. In consequat diam eget vestibulum elementum. Vestibulum in turpis gravida, accumsan libero placerat, scelerisque risus. Integer at tempor leo, a luctus purus. Vivamus dapibus placerat augue, vel euismod tellus elementum et. Vivamus interdum nisi eu mauris cursus vulputate. Vestibulum tempus tortor mi, et luctus sapien vehicula id. Curabitur in elit enim. Morbi viverra semper justo, id tempor justo dignissim quis. Cras scelerisque neque sit amet lacinia vulputate. Phasellus ultricies consectetur ex, eleifend viverra dolor consequat nec. Quisque rutrum ligula mauris, vitae viverra ante lobortis vel. Donec vel dictum mi. Praesent non vehicula nisi.

Vivamus vulputate nisi vitae sem laoreet pulvinar. Sed consequat diam diam, in tempus eros tristique et. Sed rhoncus enim vel velit mattis, et vestibulum mi euismod. Duis vel tristique velit. Phasellus lobortis venenatis felis, varius porttitor dolor consectetur quis. Nunc finibus ullamcorper neque placerat facilisis. Fusce nec ipsum eget nibh semper vulputate. Aenean sit amet leo sit amet tellus porttitor elementum eget ut risus.

Duis eleifend eros eget ullamcorper luctus. Proin ac dictum nunc, sodales viverra est. Nullam faucibus lorem felis, nec dapibus nisi imperdiet id. Proin condimentum dui at metus porta feugiat. Integer nunc est, fermentum sed leo non, cursus vehicula dolor. Vivamus dolor orci, consectetur vitae diam sit amet, pellentesque ullamcorper justo. Donec sem libero, scelerisque quis eros vitae, rhoncus egestas arcu. Vivamus congue, massa ac hendrerit condimentum, odio odio varius justo, sit amet sodales dolor lorem quis dolor. Vestibulum augue ligula, euismod ac nibh eu, laoreet fermentum mauris.

Suspendisse congue, ex sit amet gravida pulvinar, risus mauris tristique purus, rhoncus mollis neque purus pharetra dolor. Donec scelerisque nunc ac ligula dictum, ac euismod nulla accumsan. Integer id felis libero. Proin a quam ultrices ante blandit ultricies eu ac metus. Quisque sagittis malesuada dui. Donec eleifend, nisl id ullamcorper sodales, dolor enim eleifend turpis, eu ultrices augue nisl non turpis. Duis quis justo hendrerit, posuere nunc eu, condimentum odio. Phasellus viverra velit dui, eget cursus massa pellentesque eu. Phasellus dignissim orci nisl, quis lobortis ligula porta id.

Nulla sed finibus arcu. Sed malesuada, leo quis egestas porttitor, felis lorem consequat velit, quis convallis quam erat sit amet libero. Proin sed vulputate quam, sit amet auctor enim. Morbi a egestas neque, vitae suscipit eros. Morbi finibus odio quis imperdiet porttitor. Nullam condimentum mi leo, quis fringilla sapien ultrices lacinia. Cras et tristique lacus, eget tristique lacus. Donec ultricies eget ante vitae sodales. Phasellus tempor massa id elit varius, eu dictum nulla vehicula. Suspendisse ac nulla non felis aliquet finibus. Pellentesque tincidunt magna in dolor sodales tempor vel et ante. Ut tempor eu dui at gravida. Sed non ornare nunc, ac mollis felis. Sed gravida quam a tellus consectetur, id congue turpis tristique. Sed nec libero at ex consequat molestie a quis elit. Praesent auctor non nisl vel iaculis.

Nulla vehicula erat nec lorem consequat venenatis. Pellentesque purus mi, imperdiet id magna non, feugiat finibus ligula. Praesent dolor dui, varius vitae quam ac, ultricies interdum augue. Integer at laoreet orci. Nullam lorem mauris, aliquet ac tempus vitae, tempor ac enim. Aenean ut tempor orci. Suspendisse pellentesque dignissim nunc vel consectetur. Fusce et elit in nisi egestas volutpat. In hac habitasse platea dictumst. Suspendisse potenti. In hac habitasse platea dictumst. Mauris gravida tortor nibh, eget varius turpis porta vel. Integer vestibulum nisl risus, non laoreet nibh blandit et. Etiam maximus nunc vel sem placerat scelerisque. In consectetur nisl in augue laoreet, vitae volutpat sem tempus.

Nullam metus felis, vehicula vitae lacus non, euismod tincidunt mi. Praesent efficitur lobortis velit sit amet condimentum. Vestibulum gravida porta suscipit. Sed id ligula quis risus vehicula finibus. Nullam non nisi vel nisl gravida accumsan. Aenean vel porttitor leo, at tempus elit. Nulla in eros quis risus tincidunt consectetur vulputate sit amet neque. Cras ultrices erat velit, vitae auctor eros sagittis quis. Nullam et egestas tellus. Donec placerat turpis metus, sit amet ornare purus rutrum sit amet.

Phasellus elementum felis at ante dapibus hendrerit. Pellentesque at mauris et arcu consectetur tristique aliquam fringilla justo. Curabitur convallis nisl commodo, tempor sapien et, semper augue. Integer varius eget neque vitae dapibus. Etiam lobortis dui in ex luctus mollis. Pellentesque rhoncus mi rhoncus orci efficitur, eget ornare quam sollicitudin. Nulla tortor metus, laoreet at fermentum finibus, pellentesque sagittis lectus. Curabitur interdum quam erat, et porttitor risus vehicula et. Vestibulum vestibulum, leo in lacinia condimentum, arcu lorem semper leo, sit amet ornare orci turpis vel mi. Ut scelerisque eleifend bibendum. Vestibulum sed varius tortor. Vivamus ut purus eget sem sagittis iaculis.

Quisque ullamcorper fermentum nisl eu blandit. Donec consectetur diam eget iaculis bibendum. Ut viverra urna non erat faucibus, id ullamcorper augue ultrices. Sed et massa malesuada, vestibulum nibh tristique, tempor lorem. Integer luctus dolor et lorem blandit, et ullamcorper augue pharetra. In in luctus nibh. Fusce at erat risus. Quisque sed felis nulla. Pellentesque venenatis iaculis lacus, ac ullamcorper arcu pulvinar in. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Vestibulum suscipit fermentum mi vel facilisis. Sed vel dui viverra, pulvinar odio a, hendrerit ex. Aenean quis dignissim tellus.

Nunc dui nulla, convallis sit amet eros at, iaculis blandit mauris. Nunc vitae bibendum diam. Morbi scelerisque ultrices libero ut fringilla. Maecenas cursus, dui pulvinar maximus finibus, erat ipsum pulvinar mi, a pretium ligula diam nec justo. Vivamus hendrerit suscipit neque ut pharetra. Praesent quam felis, pharetra ut consequat non, sagittis non purus. Suspendisse potenti. Nullam ac metus ac nisl efficitur fermentum vitae et turpis. Nunc sit amet odio ac ipsum ornare aliquet a in enim. Pellentesque ornare laoreet risus sit amet suscipit.

Aliquam feugiat mollis nisl, in laoreet sapien tincidunt et. Fusce at enim ut urna tincidunt blandit eget vitae augue. Sed eros massa, vestibulum non facilisis in, dictum in metus. Praesent eu nibh at lorem mattis dignissim. Nam id diam vel ante tempus malesuada. Phasellus sollicitudin mollis lectus ut aliquet. Nam et sapien in sapien bibendum fringilla nec vel felis. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Maecenas elementum a dui scelerisque sodales. Mauris leo purus, lobortis id blandit sed, facilisis sit amet lacus. Curabitur vehicula ultrices vestibulum. Cras lacinia nisi ac mauris volutpat dictum. Praesent quam neque, pretium vitae euismod ac, dictum quis odio. Integer eget nulla eu mauris convallis condimentum vel eu urna. Etiam blandit porta dolor eget volutpat. Nulla facilisi.

Donec molestie enim tortor, eget dapibus mauris dapibus id. Pellentesque ligula sapien, fringilla sed eros sodales, aliquam dictum lectus. Sed sit amet vestibulum magna. In non volutpat sem, sit amet posuere massa. Aenean fermentum risus sit amet lectus euismod, et fringilla arcu semper. Sed cursus erat pulvinar, auctor lectus quis, posuere sapien. Etiam mattis tellus id leo mollis tincidunt ut eget libero.

Aliquam ac faucibus urna. Suspendisse rhoncus sodales molestie. Vestibulum id cursus nisl. Nullam non elit gravida, vehicula nibh sed, maximus sem. Etiam scelerisque lectus ante, a rutrum augue auctor ut. Cras erat dolor, mattis vel magna sit amet, finibus suscipit purus. Vivamus rhoncus ligula ut sapien vehicula auctor. Nunc malesuada finibus nisi, in sagittis eros molestie a. Curabitur nisi dui, laoreet id pharetra nec, faucibus quis quam. Vivamus in ipsum elementum justo viverra mollis. Etiam consectetur commodo nisl, sit amet sagittis nisl aliquet at. Vivamus vulputate rutrum magna, at scelerisque ligula suscipit id. In hac habitasse platea dictumst. Morbi sodales quam nec imperdiet aliquam. Suspendisse venenatis libero nec bibendum semper. Cras maximus eget tortor ut venenatis.







