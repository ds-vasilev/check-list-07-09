*В тестовом задании осталось много непонятного - от реализации функционала (будет ли у расчетов/карточки клиента фронт, либо у нас всего одно поле с выбором клиента и после выбора отображается цена КАСКО и сумма скидки, а данные для расчета тянутся из БД) и до того, суммируются ли скидки и в каком порядке.*

*По понятной мне бизнес-логике клиент при возможности получить несколько скидок, получает только самую большую (в противном случае общая скидка может дойти до 60-80%, что не логично), штрафы клиент получает всегда.*

*Для расчетов использовал логику, в которой скидка и штраф считаются от базовой стоимости КАСКО.*

*Из таких предусловий составил тест-план.*




# Тест-план:

    *проверить интерфейс в карточке клиента

    *проверить корректность ввода информации о клиенте:

        *ФИО

        *чекбоксы
    
    *проверить, что штраф за наличие ДТП учитывается всегда

    *проверить что при любом кол-ве выбранных чекбоксов со скидкой начисляется только одна, самая большая скидка

    *проверить корректность расчетов
