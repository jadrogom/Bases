# Bases
select * from usuarios;

select bibliotmp.titbib,autores.nomaut,prestamostmp.fecpre, bibliotmp.codcbi 

from bibliotmp inner join autores on 
autores.codaut= bibliotmp.codaut
inner join prestamostmp on prestamostmp.codbib= 
bibliotmp.codbib WHERE codcbi =6;



select prestamostmp.codusu,usuarios.nomusu,   bibliotmp.titbib, prestamostmp.fecpre
from bibliotmp
 inner join prestamostmp on prestamostmp.codbib= bibliotmp.codbib
inner 
join usuarios on usuarios.codusu= prestamostmp.codusu WHERE fecpre = CURRENT_DATE-40;

sentencias SQL
