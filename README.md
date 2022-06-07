# Reproducer

```bash
git clone git@github.com:alexander-schranz/symfony-reproducer-twig-global-compilerpass.git reproducer-twig-global
cd reproducer-twig-global
composer install
bin/console cache:clear
```

Errors with:

```bash
 [KO]
Script cache:clear returned with error code 1
!!
!!  In ParameterBag.php line 93:
!!
!!    You have requested a non-existent parameter "app.twig_global".
!!
!!
!!
Script @auto-scripts was called via post-install-cmd

In ParameterBag.php line 93:

  You have requested a non-existent parameter "app.twig_global".
```
